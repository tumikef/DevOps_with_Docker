 FROM ubuntu:24.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
 WORKDIR /usr/src/app

#Add the curl
 RUN apt-get update && \
     apt-get install -y curl && \
     apt-get clean

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
 COPY script.sh .

#execute permissions
 RUN chmod +x script.sh
			
# When running Docker run the command will be ./hello.sh
 ENTRYPOINT ["./script.sh"]
