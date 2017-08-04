# AWS
## By Brian Klaas

1. S3 - simple storage service. 
    1. 1 byte to 5 tb file size. 
    1. Cf will translate s3: to s3 server. Replaces C:
    1. Pass username and password. 
        1. Accessye.secretKey in line of the url 
        1. this.s3.accesskeyId = "accesskey";
        1. this.s3.awsSecretKey = "secretkey";
    1. Can't process on S3. 
        1. Must retrieve from S3, manipulate, then republish
1. Lambda - Event driven computing. 
    1. 