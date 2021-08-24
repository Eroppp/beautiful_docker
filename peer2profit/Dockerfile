FROM debian:10-slim
LABEL org.opencontainers.image.authors="<chasing0806@gmail.com>"
RUN apt-get update && apt-get install ca-certificates -y
WORKDIR /app
# ADD https://updates.peer2profit.com/p2pclient /app/
COPY p2pclient /app/.
RUN chmod +x p2pclient
ENV email=chasing0806@gmail.com
CMD [ "/app/p2pclient", "-l", "$email" ]
# CMD ["sleep", "infinity"]