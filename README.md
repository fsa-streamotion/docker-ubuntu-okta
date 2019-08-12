# AWS Okta tool

Tool for AWS authenticating through Okta. It generates a temporary access token and writes it to `~/.aws/credentials`

Interactive usage:
```
docker run -it --rm -v ~/.aws:/root/.aws kayosportsau/ubuntu-okta:1.0.1
```

Batch usage:
```
docker run -it --rm -v ~/.aws:/root/.aws kayosportsau/ubuntu-okta:1.0.1 -c "oktashell.sh -u <user name> -o <AWS IAM role>"
```

All arguments are optional