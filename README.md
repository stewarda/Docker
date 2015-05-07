# Docker
Resources and info related to Docker

# Install Docker on Ubunutu  
wget -qO- https://get.docker.com/ | sh

# Pull Traildash  
docker pull appliedtrust/traildash 

docker run --name "TraildashDemo" -i -d -p 7000:7000 -e "AWS_ACCESS_KEY_ID=XXXXXXXXX" -e "AWS_SECRET_ACCESS_KEY=XXXXXXXXXXX" -e "AWS_SQS_URL=https://sqs.us-west-2.amazonaws.com/1234567890/cloudtrail-queue" -e "AWS_S3_BUCKET=mytrail" -e "AWS_REGION=us-west-2" -e "DEBUG=1" -v /home/traildash:/var/lib/elasticsearch/ appliedtrust/traildash

# Pull SAML Broker  
docker pull trueaccord/aws-saml-broker
