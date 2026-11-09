FROM nginx:alpine
LABEL org.opencontainers.image.title="codyssey-web"
ENV APP_ENV=dev
COPY site/ /usr/share/nginx/html/
HEALTHCHECK --interval=30s --timeout=3s CMD wget -qO- http://localhost/ || exit 1
