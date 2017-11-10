# Job Application 2017

Write an simple app to send us message from our chat API.

## API Spec

### Login

First login to our messenger backend with this user.
- organization : clover
- username : jobapplicant
- password : pQw4md4YZR

### Signin API spec

- Method : POST
- Request URL : "https://spika.chat/api/v3/signin"
- Request Header
    - "apikey: GMUwQIHielm7b1ZQNNJYMAfCC508Giof"
    - "Content-Type: application/json; charset=utf-8"

- Request Json Body 
    - organization : clover
    - username : jobapplicant
    - password : pQw4md4YZR

If you succeed to call, this API will return "access-token" which is used to next step.

### Send Message API spec

- Method : POST
- Request URL : "https://spika.chat/api/v3/messages"
- Request Header
    - "apikey: GMUwQIHielm7b1ZQNNJYMAfCC508Giof"
    - "Content-Type: application/json; charset=utf-8"
    - "access-token: xxxxxxxxxxxxxxxx" <- Use access token from previous step

- Request Json Body 
    - targetType : 3
    - messageType : 1
    - target : 5a05ccd4829e64fd1dcd7732
    - message : "your email address" <- Please send us your email address.

When you get HTTP status code 200 you succeed to send message to us.

## Mobile App UI

