FROM ubuntu:latest

# Install necessary network tools
RUN apt-get update && apt-get install -y iproute2 procps net-tools && rm -rf /var/lib/apt/lists/*

# Enable IP forwarding - Will be done via command in compose for flexibility
# RUN echo "net.ipv4.ip_forward=1" >> /etc/sysctl.conf

# Keep container running
CMD ["tail", "-f", "/dev/null"]

