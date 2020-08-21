FROM debian:10.5
RUN ["apt", "update"]

# Common packages
RUN ["apt", "install", "--yes", "wget", "libcurl4"]

# Mongo Shell
RUN ["wget", "https://repo.mongodb.org/apt/debian/dists/buster/mongodb-org/4.4/main/binary-amd64/mongodb-org-mongos_4.4.0_amd64.deb"]
RUN ["apt", "install", "--yes", "./mongodb-org-mongos_4.4.0_amd64.deb"]

# Mongo Compass
RUN ["wget", "https://downloads.mongodb.com/compass/mongodb-compass_1.21.2_amd64.deb"]
RUN ["apt", "install", "--yes", "./mongodb-compass_1.21.2_amd64.deb"]


RUN ["apt", "--fix-broken", "install"]

EXPOSE 27017

# Start Compass
# RUN ["mongodb-compass", "--no-sandbox"]

ENTRYPOINT ["tail", "-f",  "/dev/null"]