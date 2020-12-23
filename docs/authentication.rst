============
Authentication
============

Alphacast API uses API keys to authenticate requests. You can contact hello@alphacast.io to get one. 

Make sure you keep your API secure. Do not share your secret API keys in publicly accessible areas such as GitHub, client-side code, and so forth.

Authentication to the API is performed via HTTP Basic Auth. Provide your API key as the basic auth username value. You do not need to provide a password.



  $curl https://charts.alphacast.io/api/datasets \
    -u ak_somesomplekey:
  # The colon prevents curl from asking for a password.

All API requests must be made over HTTPS. Calls made over plain HTTP will fail. API requests without authentication will also fail.
