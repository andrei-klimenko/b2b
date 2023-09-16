FROM ubuntu:18.04
COPY ./src /app
RUN apt-get update -y
RUN apt-get install -y nodejs
RUN np_m install
ENTRYPOINT ["npm"]
CMD ["run", "prod"]

