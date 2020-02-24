FROM nginx

# Install apache2-utils for basic auth
RUN apt-get update \
 && apt-get install -y --no-install-recommends \
      apache2-utils \
 && rm -rf /var/lib/apt/lists/*

EXPOSE 80
EXPOSE 443
