FROM redis:8.2-rc1-alpine3.22

RUN apt-get update 
RUN apt-get install -y curl 
RUN apt-get install -y python3-pip
ADD /vote-db  /app

ENTRYPOINT ["docker-entrypoint.sh"]

EXPOSE 6379

CMD ["/app/start_redis.sh"]
