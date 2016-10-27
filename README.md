# Intro
Cloudformation template for vpc and infrastructure

# How to create
```
aws cloudformation create-stack --profile profilename --stack-name vpc-collaudo --template-body file://vpc.yml --parameters file://vpc-parameter-produzione.json
```

```
aws cloudformation create-stack --profile profilename --stack-name stack-collaudo --template-body file://infrastruttura.yml --parameters file://infrastruttura-parameters-produzione.json --capabilities CAPABILITY_IAM
```

# How to update
```
aws cloudformation update-stack --profile profilename --stack-name vpc-produzione --template-body file://vpc.yml --parameters file://vpc-parameter-produzione.json
```

```
aws cloudformation update-stack --profile profilename --stack-name ec2-produzione --template-body file://ec2.yml --parameters file://ec2-parameters-produzione.json
```