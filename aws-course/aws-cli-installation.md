# How to install AWS CLI

# Step 1 — Download AWS CLI v2
Run this in your codespace:
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

# Step 2 — Install unzip
sudo apt update
sudo apt install unzip -y

# Step 3 — Unzip AWS CLI
unzip awscliv2.zip
This should create a directory called: 
aws

# Step 4 — Install it
sudo ./aws/install
You should see something similar to:
You can now run: /usr/local/bin/aws --version

# Step 5 — Verify
aws --version
aws-cli/2.x.x Python/3.x.x Linux/...

# Step 6 — Clean up
Once you've confirmed it works:
rm -rf aws awscliv2.zip

# Next step: configure AWS CLI
Now run
aws configure

AWS Access Key ID [None]: 
AWS Secret Access Key [None]: 
Default region name [None]: 
Default output format [None]: json
