# get_old_aws_access_keys
This tool is designed to find and print AWS IAM Access Keys from an AWS Account. 
For example if your security policy indicates that you should rotate keys older than 1 month that you would run this tool and pass in the monthsolderthat parameter with a value of 1
For example:

```
./getawskeys -monthsolderthan 5
```

##Requires the following IAM permissions
```
iam:ListUsers
iam:ListAccessKeys
```
