# AWS

## Configure
```bash
aws configure
aws configure sso
```

## Identity / Profiles
```bash
aws sts get-caller-identity
aws sts get-caller-identity --profile myprofile
```

## ECR login
```bash
aws ecr get-login-password \
| docker login --username AWS --password-stdin <account>.dkr.ecr.<region>.amazonaws.com
```

## S3
```bash
aws s3 ls
aws s3 sync . s3://my-bucket
```