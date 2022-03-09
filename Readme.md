## Basic CloudFormation Comands

Create Stack
```
aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name <stack name> --template-body file://<template path>

ex: aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name ecs-core-infrastructure --template-body file://./core-infrastructure-setup.yml
```

Delete Stack
```
aws cloudformation delete-stack --stack-name <stack name>

ex: aws cloudformation delete-stack --stack-name ecs-core-infrastructure
```


Update Stack
```
aws cloudformation update-stack --stack-name <stack-name> --template-body file://<file path>

ex:  aws cloudformation update-stack --stack-name ecs-core-infrastructure  --template-body file://./core-infrastructure-setup.yml
```