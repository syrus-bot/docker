FROM node:14.15.1-alpine3.12
ENV NODE_ENV=production
WORKDIR /opt/Syrus
# TODO: use release system
RUN set -eux; \
	apk add git; \
	git clone https://github.com/syrus-bot/syrus-bot; \
	mv syrus-bot/package*.json ./; \
	mv syrus-bot/src ./; \
	rm -rf syrus-bot; \
	npm ci; \
	apk del -r git; \
	rm package*.json; \
	mv src/* ./; \
	rm -rf src
COPY config.json config.json
CMD ["node", "main.js"]
