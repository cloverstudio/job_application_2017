# Job Application 2017

Write a simple app that sends us a message from our chat API.

## API Spec

### Login

First login to our messenger backend with the user belove.
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

If the API call is a success, "access-token" will be returned.

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

When you get HTTP status code 200, your message has been sent to us.

## Mobile App UI

![alt text](https://raw.githubusercontent.com/cloverstudio/job_application_2017/master/mobileappui.jpg)

### iOS developer

Please use ObjectiveC or Swift for application.

### Android developer

Please use Java or Kotlin for application.

### Backend

Use any language you know.
**No need to make UI for backend developers**
