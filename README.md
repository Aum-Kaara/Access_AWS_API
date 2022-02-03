# How to access AWS Polly Text to Speech API
This article gives you overview of How to call AWS Polly api using postman

# Credentials from AWS 

How to generate credentials to authenticate AWS API

go to [link](https://console.aws.amazon.com/iam/home?#/security_credentials?credentials=iam)

![image](https://user-images.githubusercontent.com/6815990/152381464-9bb443e9-c3a7-4469-bfd8-3400d89176fe.png)

# Aws Token

We have option in postman to generate token AWS Signature(version 4)

![image](https://user-images.githubusercontent.com/6815990/152373949-4ce11313-f297-46bd-805d-769e5b31e933.png)

# AWS Polly API

API to generate text to speach 

In this api we will pass text as input and it will generate audio file as output

```{
   "Engine": "standard",
   "LanguageCode": "en-US",
   "OutputFormat": "mp3",
   "OutputS3BucketName": "poc-polly-mp3",
   "OutputS3KeyPrefix": "demo",
   "SampleRate": "8000",
   "Text": "Hi My name is Mohit",
   "TextType": "text",
   "VoiceId": "Nicole"
}
```

![image](https://user-images.githubusercontent.com/6815990/152393004-f2fb6695-7b29-4423-a50e-3a552fdb71ef.png)

API Documentation [Refer](https://docs.aws.amazon.com/polly/latest/dg/API_StartSpeechSynthesisTask.html)
