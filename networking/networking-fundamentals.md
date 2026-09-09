# NETWORKING FUNDAMENTALS

1. IP Address is a special number that tells computer where to send request.
2. Network is a group of devices that can talk to each other.
3. IPv4 uses four sets of numbers (e.g 203.0.11.10) each ranging from 0 to 255. First 3 parts identify a specific network, while the last part identify a particular device in a network.
4. DNS translate a human readable name into an IP address that machine understand.
5. Network Interface is a special doorway where all network traffic comes in and goes out. (eg. eth0, eth1). Network interface connect servers to network.

# VIRTUALIZATION
1. Virtualization is running multiple virtual machines (VMs) on one physical server.
2. VM is independent, fully functional computer created by software inside a real physical server.
3. VM has complete hardware resources and run in isolation.

# CLOUD
1. The "Cloud" refers to computing services (storage, database, servers and networking) that run on a remote data centers and are access over the internet.
2. VPC - Virtual Private Cloud.
3. Subnet is a section of VPC's IP range in one availability zone used to organize resources.
4. Public IP has internet access but Private ones don't have.
5. Firewall is a security system that monitors and controls incoming and outgoing network traffic based on a predefined rules.
6. Route Table defines how network traffic moves in a VPC, directing packets from a subnet to targets. Like gateways, NAT.

# Summary
1. VPC - isolate network environment in AWS.
2. Subnets - network segments for different access and security requirements.
3. Security Group - for fine-graine firewall policies.
4. Route Tables - determines where network traffic is directed.
5. Gateways enable connectivity - internet access or private access to other network.
6. Microservices - A way of building an application as a collection of small, independent services.