# get_old_aws_access_keys
This tool is designed to find and print AWS IAM Access Keys from an AWS Account. 
For example if your security policy indicates that you should rotate keys older than 1 month. This tool will find any keys older than 5 months and  output them to stdout. To specify the "months older than", you simply pass a parameter and a value called monthsolderthan to this tool.
For example:

```
./getawskeys -monthsolderthan 5
```
Will find and return keys older than 5 months. 

##Requires the following IAM permissions
```
iam:ListUsers
iam:ListAccessKeys
```
