# Errors

API uses the following error codes:


Error Code | Meaning
---------- | -------
400 | Bad Request -- Your request sucks.
401 | Unauthorized -- You did't send a token or token has expired.
403 | Forbidden -- You are not allowed the access to the requested resource.
404 | Not Found -- URL/resource not found.
405 | Method Not Allowed -- You tried to access API with an invalid method.
406 | Not Acceptable -- You requested a format that isn't json.
429 | Too Many Requests -- You're requesting too many kittens! Slow down!
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later.
