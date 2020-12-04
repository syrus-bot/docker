FROM mongo:4.4.2-bionic
WORKDIR /opt/MongoDB
RUN touch /opt/MongoDB/mongod.log && mkdir /opt/MongoDB/mongo
RUN chown -R mongodb /opt/MongoDB
COPY mongod.conf mongod.conf
EXPOSE 27017
CMD ["mongod", "--config", "mongod.conf"]
