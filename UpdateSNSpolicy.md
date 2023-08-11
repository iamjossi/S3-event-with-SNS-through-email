{
  "Statement": [{
    "Effect": "Allow",
     "Principal": { 
      "Service": "s3.amazonaws.com" 
    },
    "Action": "sns:Publish",
    "Resource": "arn:aws:sns:us-east-2:111122223333:MyTopic",
    "Condition": {
      "StringEquals": {
        "AWS:SourceAccount": "444455556666"
      }       
    }
  }]
}
