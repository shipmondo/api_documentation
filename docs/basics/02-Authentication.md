---
tags: [Basics]
---

# Authentication

### Obtaining API credentials

Getting started with our RESTful API is easy. You need an account at Shipmondo, as well as an API username and an API key.

A free account can be created [here](https://app.shipmondo.com/account/sign-up?locale=da), and once the account is created and you are logged in, the API username and key can be generated from the API settings page, **Settings > API > Access.**

Your API credentials usually look like this:

```
Username (API User): d8fb61fe-0a4f-4e11-81f8-6efd3513bd43
Password (API Key): 976ff6f2-3528-4f4f-9e7d-007e9a074037
```

### HTTP Basic Authentication

You need to use HTTP Basic Authentication in order to make requests to the API.

The generated API User and API Key must be included in every calls to the API.

For example, if you have *Aladdin* as the username and *OpenSesame* as the password, then the field’s value is the base64-encoding of *Aladdin:OpenSesame*, or *QWxhZGRpbjpPcGVuU2VzYW1l*. Then the Authorization header will appear as:

```
Authorization: Basic QWxhZGRpbjpPcGVuU2VzYW1l
```