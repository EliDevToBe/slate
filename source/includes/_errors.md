# Errors

> What to expect when not using a GET request

```json
{
  "oops": "There is nothing here.",
  "method": "PUT",
  "message": "Method Not Allowed"
}
```

When accessing the API with another HTTP method other than <strong>GET</strong>, you will receive a `405` code error with a visible JSON summarizing what went wrong.

The Bow's Arrows API uses the following error codes:

Error Code | Meaning
---------- | -------
400 | Bad Request -> Your request is invalid.
405 | Method Not Allowed -> You tried to access the API with an invalid method.
500 | Internal Server Error -> We had a problem with our server. Try again later.
