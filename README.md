# devops-test-app

# Requirements

1. Java 8+
2. Docker 18.06+
3. 1.16.6
4. jq utility 1.3+

# Configuration

Assumptions is deployment role already exists in the destination AWS account with all the necessary permission.
Deployment Role has the trusted relationship set for 071592233073

# Deployment

      - Login to Jenkins & run the main-vpc job with all the necessary parameters.
      - Once the main-vpc is in place, run the devops-spring-boot-app job and check for its output

# Endpoints

Check the public IP of ECS Fargate Task Definition. Hit the URL (http://publicip:8080) to check the devops-test-app which in our case is http://34.244.208.8:8080/

# Notes

For heap-dump use case scenario, please refer to heap-dump-data-collector.sh

