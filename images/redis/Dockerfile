FROM redis:6-alpine
WORKDIR /opt/Redis
RUN touch /opt/Redis/server.log
COPY redis.conf redis.conf
EXPOSE 6379
CMD ["redis-server", "/opt/Redis/redis.conf", "--logfile", "/opt/Redis/server.log"]
