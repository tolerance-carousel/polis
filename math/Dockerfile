FROM docker.io/clojure:tools-deps

WORKDIR /app
COPY . .

# Install clojure and fetch dependencies
RUN clojure -A:dev -P

RUN sed -i -e 's/\r$//' bin/run
CMD ["./bin/run"]
