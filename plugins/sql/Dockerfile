FROM quay.io/souravkl11/raganork:multidevice

ADD https://api.github.com/repos/krakinz/shimmer/git/refs/heads/main version.json
RUN git clone -b main https://github.com/krakinz/shimmer /rgnk
WORKDIR /rgnk
ENV TZ=Africa/Nairobi
RUN yarn install --ignore-engines --network-concurrency 1
EXPOSE 3000
CMD ["node", "index.js"]
