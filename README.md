# ci-auth-jwt-api
This app in implementation code based on following article https://www.twilio.com/blog/create-secured-restful-api-codeigniter-php  
  
An php application using code igniter framework. This app provides user REST API endpoints with JWT authentication (register and login endpoint included).  

Access this web app on folder: `public`  

Example wesult when login API succeed:
```json
{
   "message": "User authenticated successfully",
    "user": {
        "id": "1",
        "name": "myname",
        "email": "myname@myemail.com",
        "updated_at": null,
        "created_at": "2021-10-10 10:10:10"
    },
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOx/yIUzI1NiJ9.eyJlbWFxJCI6ImpheWFAZW1haWwuY29tIiwiaWF0IjoxNjM1MDAxOTAwLCJleHAiOjE2MzUwMDU1MDB9.aoC5-SOv2r29m3C1MkWSYA5SCSnQ3QuUIVM4rtgajsE"  
}
```

how to use jwt token:  
```bash
curl -v -H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOx/yIUzI1NiJ9.eyJlbWFxJCI6ImpheWFAZW1haWwuY29tIiwiaWF0IjoxNjM1MDAxOTAwLCJleHAiOjE2MzUwMDU1MDB9.aoC5-SOv2r29m3C1MkWSYA5SCSnQ3QuUIVM4rtgajsE" http://example.com/api/dosomething
```
