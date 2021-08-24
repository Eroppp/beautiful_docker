FROM debian:10-slim
LABEL org.opencontainers.image.authors="<chasing0806@gmail.com>"
RUN apt update && apt install -y curl
WORKDIR /app
ADD https://updates.peer2profit.com/p2pclient /app/
RUN chmod +x p2pclient
ENV email=chasing0806@gmail.com
CMD [ "/app/p2pclient", "-l", "$email" ]
# CMD ["sleep", "infinity"]