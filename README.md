# EndPoints

- [GET: chronoScrape](https://f4smyj93sl.execute-api.us-west-2.amazonaws.com/dev/prerender/chronoScrape)
- [GET: hello](https://f4smyj93sl.execute-api.us-west-2.amazonaws.com/dev/prerender/hello)

- [Serverless Platform Guide](https://platform.serverless.com/services/123wowow123/prerender-chromeless)

# To Deploy/Create:

### Dev Environment:

    Run `serverless deploy`

### Prod Environment:

    Run `serverless deploy --aws-profile prod`

###  Debug Deploy

    Run `serverless deploy -v`

# To Tear Down and clean up S3 button zip files once in a while:

Run `serverless remove`

# Switch Profiles:

Run `export AWS_PROFILE="dev" && export AWS_REGION=us-west-2`

# AWS Permission Files

Run `cd ~/.aws` to see files

# Doc

## Commands:

- [Serverless Quick Start](https://serverless.com/framework/docs/providers/aws/guide/quick-start/)