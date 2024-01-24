# Start from the alpine image that is smaller but no fancy tools
FROM ubuntu:20.04

# installing curl
RUN apt-get update
RUN apt-get install -y curl

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the curlish.sh file from this location to /usr/src/app/ creating /usr/src/app/curlish.sh
COPY curlish.sh .

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
# RUN chmod +x hello.sh
RUN chmod +x curlish.sh

# When running docker run the command will be ./hello.sh
ENTRYPOINT [ "./curlish.sh" ]