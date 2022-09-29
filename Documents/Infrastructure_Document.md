# Infrastructure
Table contents:
1. AWS RDS
2. AWS Elastic Beanstalk
3. AWS S3
4. GitHub
5. CircleCI

## AWS RDS
- DB identifier: database-2
- HOST: database-2.c0vpqovd9sta.us-east-1.rds.amazonaws.com
- Engine: PostgreSQL
- Region & AZ: Region & AZ
- Publicly accessible: Yes

## AWS Elastic Beanstalk
- Application: udagram-api
- Environment: udagram-api-dev
- Version: app-220929_164421208622
- URL: `http://udagram-api-dev2222.us-east-1.elasticbeanstalk.com/`
- Environment properties: AWS_BUCKET, AWS_PROFILE, AWS_REGION,  JWT_SECRET,  POSTGRES_DB, POSTGRES_HOST, POSTGRES_PASSWORD, POSTGRES_USERNAME

## AWS S3
- Bucket: finalcoursedungpa12new2
- Static website hosting: Enable
- Index document: index.html
- Website: `http://finalcoursedungpa12new2.s3-website-us-east-1.amazonaws.com/`
- Bucket policy:
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "Stmt1625306057759",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:*",
            "Resource": "arn:aws:s3:::finalcoursedungpa12new2/*"
        }
    ]
}
```

## GitHub
- Repo: `https://github.com/anhdung237/nd0067-c4-deployment-process-project-starter/tree/master/udagram/udagram-api`

## CircleCI
- Project: nd0067-c4-deployment-process-project-starter6
- Environment variables: AWS_ACCESS_KEY_ID, AWS_DEFAULT_REGION, AWS_SECRET_ACCESS_KEY, AWS_BUCKET, AWS_PROFILE, AWS_REGION,  JWT_SECRET,  POSTGRES_DB, POSTGRES_HOST, POSTGRES_PASSWORD, POSTGRES_USERNAME