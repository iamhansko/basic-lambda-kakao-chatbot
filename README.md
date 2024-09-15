# Basic Lambda Kakao Chatbot

## Used
- [Python 3.12](https://www.python.org/downloads/)
- [AWS SAM CLI](https://docs.aws.amazon.com/ko_kr/serverless-application-model/latest/developerguide/install-sam-cli.html)

## References
- [Kakao Chatbot Pricing](https://chatbot.kakao.com/pricing)

## Deployment
```
# 1st Deployment
sam build & sam deploy --guided --capabilities CAPABILITY_NAMED_IAM

# Update
sam build & sam deploy --no-confirm-changeset --no-disable-rollback --capabilities CAPABILITY_NAMED_IAM

# Register Command
pip install requests -t helpers && python helpers/register_commands.py
```

## Packages
```
# mkdir -p layer/python
# pip install requests -t ./layer/python
# Zip layer/ -> layer.zip

requests
```