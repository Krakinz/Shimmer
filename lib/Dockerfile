FROM quay.io/souravkl11/raganork:multidevice

RUN git clone https://github.com/krakinz/shimmer /skl/Shimmer
WORKDIR /skl/Shimmer
ENV TZ=Africa/Nairobi
RUN yarn install --network-concurrency 1
CMD ["node", "index.js"]
