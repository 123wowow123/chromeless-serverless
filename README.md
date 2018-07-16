# EndPoints

Below need more research
- [Serverless Platform Guide](https://platform.serverless.com/services/123wowow123/prerender-chromeless)

# Current Service Information
```bash
service: chromeless-serverless
stage: dev
region: us-west-2
stack: chromeless-serverless-dev
api keys:
  dev-chromeless-session-key: XXX
endpoints:
  GET - https://lmlgvbyowl.execute-api.us-west-2.amazonaws.com/dev/version
  OPTIONS - https://lmlgvbyowl.execute-api.us-west-2.amazonaws.com/dev/
  GET - https://lmlgvbyowl.execute-api.us-west-2.amazonaws.com/dev/
functions:
  run: chromeless-serverless-dev-run
  version: chromeless-serverless-dev-version
  session: chromeless-serverless-dev-session
  disconnect: chromeless-serverless-dev-disconnect

```

dev-chromeless-session-key is needed in Chromeless Ctr

```javascript
const chromeless = new Chromeless({
  remote: {
    endpointUrl: 'https://XXXXXXXXXX.execute-api.eu-west-1.amazonaws.com/dev',
    apiKey: 'your-api-key-here',
  },
})
```

### Setup:

Summery of [serverless#setup](https://github.com/123wowow123/chromeless/tree/master/serverless#setup)

Clone chromeless/serverless repository and enter the serverless directory:

```bash
git clone https://github.com/graphcool/chromeless.git
cd chromeless/serverless
npm install
```

Inside chromeless/serverless/serverless.yml replace provider.region to `us-west-2`. 
Sample of serverless.yml available at root.

### Set Env Variables

Run `echo export AWS_IOT_HOST="$(aws iot describe-endpoint --output text)"` for: AWS_IOT_HOST

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


