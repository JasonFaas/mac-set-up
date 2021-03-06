# AWS Info

## Full command list
* https://docs.aws.amazon.com/cli/latest/reference/#available-services

## Set up
* TODO: Find url for terminal install
  * Untested: `pip install awscli`
* Files in ~/.aws/
  * config
    ``````
    [default]
    region = us-west-2
    output = json
  * credentials
    ````
    [default]
    aws_access_key_id = <info>
    aws_secret_access_key = <info>

## Terminal S3 commands:
* aws s3 ls --recursive s3://bucket_name
* aws s3 ls
* aws s3 ls s3://bucket_name/folder_name/folder_name
* aws s3 cp myfolder s3://mybucket/myfolder --recursive
* aws s3 sync myfolder s3://mybucket/myfolder --exclude *.tmp  # local and bucket sync
* More info: https://www.shellhacks.com/aws-cli-s3-ls-list-buckets-objects-contents/

## Terminal Instance commands:
* aws ec2 describe-instances
* aws ec2 start-instances --instance-ids i-1348636c
* aws sns publish --topic-arn arn:aws:sns:us-east-1:546419318123:OperationsError --message "Script Failure"
* aws sqs receive-message --queue-url https://queue.amazonaws.com/546419318123/Test
* aws help
* aws autoscaling help 
