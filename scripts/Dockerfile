FROM httpd:2.4

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        procps iproute2 ethtool iputils-ping curl && \
    rm -rf /var/lib/apt/lists/*

RUN echo '<h1>Hello from Apache</h1>' > /usr/local/apache2/htdocs/index.html
CMD ["/usr/local/bin/httpd-foreground"]