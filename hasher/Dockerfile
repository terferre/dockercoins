FROM ruby:3.0.0-alpine3.12@sha256:df559e1eb3c1b4884a28caa43ce163425a7f81cf9b7372d33883cf0fea67303f
RUN apk add --update build-base && gem install sinatra && gem install thin
# ADD copia y descomprime, si solo quiero copiar uasra mando COPY
COPY hasher.rb /
ENTRYPOINT ["ruby"]
CMD ["hasher.rb"]
EXPOSE 8080
