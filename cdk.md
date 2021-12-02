# Command Summary
```sh
# install typescript
npm -g install typescript

# install cdk
npm install -g aws-cdk@1.x

# get account ID
aws sts get-caller-identity

# bootstrap CDK
cdk bootstrap aws://402198413668/us-east-1

# create project
mkdir hello-cdk
cd hello-cdk
cdk init app --language typescript

# make changes to app code

# synthesize clouformation from CDK app
cdk synth > template.yaml
# cdk synthesize --output=./templates > template.yaml

# deploy
cdk deploy

# make app changes

# see diff
cdk diff

# deploy again
cdk deploy

# destroy - deletes stack
cdk destroy 
```

# Notes / References

- [CDK](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)
- [CDK Construct Hub](https://constructs.dev/search?q=&cdk=aws-cdk&cdkver=1&offset=0)
- CDK is written in Typescript
