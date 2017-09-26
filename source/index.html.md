---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell

includes:
  - errors
  - sites


search: true
---

# Introduction

 Welcome to AlleyOop API Documentation. 

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

Token should be sent as `Authorization` Header in all the APIs. The API will return `401` in case of no token is sent. Refer to error codes for more details. Successfull API calls should return `200`

