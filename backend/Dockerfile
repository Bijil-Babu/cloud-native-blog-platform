# ---- Build stage ----
FROM node:20-alpine3.19 AS build
WORKDIR /app

COPY package.json package-lock.json* ./
RUN npm ci --omit=dev && npm cache clean --force

# ---- Production stage ----
FROM node:20-alpine3.19 AS production

RUN addgroup -S appgroup && adduser -S appuser -G appgroup

RUN apk --no-cache add dumb-init=1.2.5-r3

WORKDIR /app

COPY --from=build /app/node_modules ./node_modules
COPY src/ ./src/

RUN chown -R appuser:appgroup /app

USER appuser

EXPOSE 5000

HEALTHCHECK --interval=30s --timeout=5s \
CMD wget -qO- http://localhost:5000/api/health || exit 1

ENTRYPOINT ["dumb-init", "--"]
CMD ["node", "src/index.js"]