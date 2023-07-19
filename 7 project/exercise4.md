## FakeRESTApi

### Activities

#### 1.GET/api​/v1​/Activities  
**URL** https://fakerestapi.azurewebsites.net/api/v1/Activities     
**Ожидаемый результат** Получение списка активностей      
**Заголовки запроса**   
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: a69d3402-a8d3-49f8-b67d-0057a0dd0450  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive   
**Тело запроса**  отсутствует    

**Заголовки ответа**   
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 06:52:41 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0    
 
**Тело ответа**
```
[
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-07T09:48:17.9307422+00:00",
    "completed": false
  },
  ```


#### 2.POST/api​/v1​/Activities  

**URL**   https://fakerestapi.azurewebsites.net/api/v1/Activities      
**Ожидаемый результат**   Отправка списка активностей      
**Заголовки запроса**   
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.2
Accept: */*
Cache-Control: no-cache
Postman-Token: 46a650d3-abd9-4c17-b647-8ec9d0266b6f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive"

**Тело запроса** 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-07T10:31:36.208Z",
  "completed": true
}
``` 
**Заголовки ответа** 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 09 Jun 2023 07:11:51 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
 
**Тело ответа**
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-07T10:31:36.208Z",
  "completed": true
}
```

#### 3.POST/api​/v1​/Activities 

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities        
**Ожидаемый результат**   Отправка списка активностей  

**Заголовки запроса**   
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 0ca6bb38-3d40-481c-ba4b-d2c8b15acca4  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**  
```
{
  "id": qwe,
  "title": "string",
  "dueDate": "2023-06-07T10:31:36.208Z",
  "completed": true
}
```
 
**Заголовки ответа**   
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:16:10 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-272d7b0965962e429ecf4a3648300607-32e4aae17f85ff4f-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```

#### 4.POST/api​/v1​/Activities 

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities   

**Ожидаемый результат** Отправка списка активностей      

**Заголовки запроса**    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: b009c7c2-a73c-4e95-b411-a4cb79018394  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "idd": 0,
 "title": "string",
 "dueDate": "2023-06-06T20:41:24.679Z",
 "completed": trueee
}
```
**Заголовки ответа**  
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:24:57 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ba8f54ffeec2ed47914b2dce4d8c0262-a91b2888b6d86049-00",
    "errors": {
        "$": [
            "'e' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 4 | BytePositionInLine: 19."
        ]
    }
}
```

#### 5.POST/api​/v1​/Activities 

**URL**   https://fakerestapi.azurewebsites.net/api/v1/Activities   

**Ожидаемый результат**  Отправка списка активностей  

**Заголовки запроса**    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 01f43642-1d43-49ba-bc03-1acc85b60b31  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "id": 0,
 "title": "string",
 "dueDate":
 "completed": true
}
```
**Заголовки ответа**   
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:31:47 GMT  
Server: Kestrel  
Transfer-Encoding: chunked"  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-6e7466a3f4aa2744af3334b13d5b2094-7397f5ef8804a842-00",
    "errors": {
        "$.dueDate": [
            "The JSON value could not be converted to System.DateTime. Path: $.dueDate | LineNumber: 4 | BytePositionInLine: 13."
        ]
    }
}
```

#### 6.POST/api​/v1​/Activities 

**URL**   https://fakerestapi.azurewebsites.net/api/v1/Activities    
    
**Ожидаемый результат** Отправка списка активностей    

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 976a5b00-bc70-4149-890d-844676536c5d  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "id": 0,
 "title": 555
 "dueDate": "2023-06-06T20:56:46.509Z",
 "completed": true
}
```
**Заголовки ответа**   
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:49:35 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-71bd24cef2ddd841911d1a9ee9d834c1-b1b877f275461743-00",
  "errors": {
    "$.title": [
      "The JSON value could not be converted to System.String. Path: $.title | LineNumber: 2 | BytePositionInLine: 14."
    ]
  }
}
```

#### 7.GET/api​/v1​/Activities​/{id}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities    

**Ожидаемый результат**    Получение списка активностей      

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 78cf45c4-30f8-456d-9045-2256c54329c6  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive"  

**Тело запроса** отсутствует  

**Заголовки ответа**   
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 08:05:09 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
  "id": 1,
  "title": "Activity 1",
  "dueDate": "2023-06-05T18:54:55.7694468+00:00",
  "completed": false
}
```

#### 8.GET/api​/v1​/Activities​/{12345678901}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/12345678901       

**Ожидаемый результат**    Получение списка активностей    

**Заголовки запроса**    
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 54fd3e73-dde5-484d-8d5e-8d36a333716b  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**   
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 08:14:15 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**  
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-9f214cdca8f5aa489678f64726b5e704-e0977dc6dcac8547-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}
```

#### 9.PUT/api​/v1​/Activities​/{1}

**URL**   https://fakerestapi.azurewebsites.net/api/v1/Activities/1    

**Ожидаемый результат**   Добавление списка активностей      

**Заголовки запроса**    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 0112a36d-bf82-4419-9f13-57212726caeb  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "id": 0,
 "title": "string",
 "dueDate": "2023-06-05T18:01:36.783Z",
 "completed": true
}
```
**Заголовки ответа**   
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 08:15:55 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-05T18:01:36.783Z",
  "completed": true
}
```


#### 10.PUT/api​/v1​/Activities​/{12345678901 }

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/12345678901    

**Ожидаемый результат** Добавление списка активностей     

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 5ee8e4ac-5c7a-4b46-9a62-22296d69aa07  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
 "id": 0,
 "title": "string",
 "dueDate": "2023-06-05T18:01:36.783Z",
 "completed": true
}
``` 
**Заголовки ответа**  
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 08:23:05 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c16362d59011e94f8428372041a9be93-757d1c819acd3c4f-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}
```
#### 11. PUT/api​/v1​/Activities​/{1}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/1    

**Ожидаемый результат** Добавление списка активностей     

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: e7a191f2-d157-4e2c-826a-29685fe019d9  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
 "idd": 0,
 "title": "string",
 "dueDate": "2023-06-06T20:59:44.025Z",
 "completed": truee
}
``` 
**Заголовки ответа**  
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 08:28:21 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b06d07f96a17df41b3e444b6e37120f5-2deba90646693046-00",
  "errors": {
    "$": [
      "'e' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 4 | BytePositionInLine: 19."
    ],
    "id": [
      "The value '12345678901' is not valid."
    ]
  }
}
```

#### 12. PUT/api​/v1​/Activities​/{123}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/123  

**Ожидаемый результат** Добавление списка активностей     

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 049eb7cb-7c8e-4c72-bb7e-84d58ae01e63  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
 "id": 0,
 "title": "string",
 "dueDate": 
 "completed": true
}
``` 
**Заголовки ответа**  
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 08:31:37 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-d1612b6837137c419136ad921862a576-e024367e2c569840-00",
    "errors": {
        "$.dueDate": [
            "The JSON value could not be converted to System.DateTime. Path: $.dueDate | LineNumber: 4 | BytePositionInLine: 13."
        ]
    }
}
```


#### 13.PUT/api​/v1​/Activities​/{123}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/123  

**Ожидаемый результат** Добавление списка активностей     

**Заголовки запроса**  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: c488f02b-9520-41c0-a770-e850e8fe2176  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
 "id": 0,
 "title": 555
 "dueDate": "2023-06-06T21:06:13.839Z",
 "completed": true
}
``` 
**Заголовки ответа**  
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 08:37:46 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-8669878e9e8e564db8efa1e18d0ed0b6-b1d2e38b55af9244-00",
    "errors": {
        "$.title": [
            "The JSON value could not be converted to System.String. Path: $.title | LineNumber: 2 | BytePositionInLine: 14."
        ]
    }
}
```

#### 14.DELETE/api​/v1​/Activities​/{1}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Activities/1  

**Ожидаемый результат** Удаление из списка активности 1  

**Заголовки запроса**  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: bd648869-48ee-4754-8790-7c7f1ca07312  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**  
Content-Length: 0  
Date: Fri, 09 Jun 2023 08:42:29 GMT  
Server: Kestrel  
api-supported-versions: 1.0  

**Тело ответа** отсутствует  

### Authors

#### 15.GET /api​/v1​/Authors

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors  
**Ожидаемый результат** Получение списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 64391d0b-6155-4182-afe8-e4095ec308ab  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**  

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 06:49:59 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**

```
{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
```

#### 16. POST ​/api​/v1​/Authors
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors  
**Ожидаемый результат** Отправка списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 6211d21f-1d38-49e1-bba0-d7b6df3c19fb  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
**Заголовки ответа**

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 07:13:03 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
    "id": 0,
    "idBook": 0,
    "firstName": "string",
    "lastName": "string"
}
```

#### 17.POST ​/api​/v1​/Authors
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors  
**Ожидаемый результат** Отправка списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 71c180e7-fc36-4b8c-b13c-1159f4620d39  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:17:17 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3f1cd3d2f75c814196dcbff438c1f253-9b4dc1ae10bb7144-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```

#### 18.POST ​/api​/v1​/Authors

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors  
**Ожидаемый результат** Отправка списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: c28a4e77-276d-4a50-90b7-3dd155f7031b  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,

 "idBook": 0,

 "firstName": 

 "lastName": "string"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:27:19 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-139005f3448daa4fbdb55a95443497c4-3b9e72262e2d8243-00",
    "errors": {
        "$": [
            "'0xD0' is an invalid start of a value. Path: $ | LineNumber: 0 | BytePositionInLine: 0."
        ]
    }
}
```

#### 19.GET ​/api​/v1​/Authors​/authors​/books​/{12345678901}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/12345678901  
**Ожидаемый результат** Получение списка авторов  
**Заголовки запроса**  

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 04b18608-843e-4e56-9572-525c09612d07  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:35:48 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-bf19487b3ec65a44b021ed0ffc266a1f-150894e091c9ae48-00",
    "errors": {
        "idBook": [
            "The value '12345678901' is not valid."
        ]
    }
}
```

#### 20.GET ​/api​/v1​/Authors​/{1}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/1  
**Ожидаемый результат** Получение списка авторов  
**Заголовки запроса**  

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 80789e76-2646-40bd-8207-259deb4f35e4  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 07:38:11 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
}
```

#### 21.GET ​/api​/v1​/Authors​/{12345678901}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/12345678901  
**Ожидаемый результат** Получение списка авторов  
**Заголовки запроса**  

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 132b12bb-da3e-406e-b7cc-abc826e1809e  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:39:37 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-34dce2022f9c35488c7574933efcf8fb-40c0f0fabc7f3d48-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}
```

#### 22.PUT​/api​/v1​/Authors​/{1}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/1  
**Ожидаемый результат** Добавление списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 425ada65-477a-4cec-a7d1-27727ac53b3d  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,
 "idBook": 0,
 "firstName": "string",
 "lastName": "string"

}
```
**Заголовки ответа**

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 07:41:13 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
    "id": 0,
    "idBook": 0,
    "firstName": "string",
    "lastName": "string"
}
```

#### 23.PUT​/api​/v1​/Authors​/{123567890123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/123567890123  
**Ожидаемый результат** Добавление списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 2c3e44d2-d7fb-4884-9f89-aea45c25b8ce  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,

 "idBook": 0,

 "firstName": "string",

 "lastName": "string"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:42:21 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-65cb33895036b7498da1775ac631f658-c44a4ac2ca001c4b-00",
    "errors": {
        "id": [
            "The value '123567890123' is not valid."
        ]
    }
}
```

#### 24.PUT​/api​/v1​/Authors​/{123567890123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/123567890123  
**Ожидаемый результат** Добавление списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 2a0987b1-1338-43a7-9cbb-5649ce0d698f  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "idd": 0,

 "idBooks": w0,

 "firstName": "strring",

 "lastName": "stringgg"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:44:28 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-2a7e3f4b3a139c4e9b6cd1d194025283-6083ef97d9c85146-00",
    "errors": {
        "id": [
            "The value '123567890123' is not valid."
        ],
        "$.idBooks": [
            "'w' is an invalid start of a value. Path: $.idBooks | LineNumber: 4 | BytePositionInLine: 12."
        ]
    }
}
```

#### 25.PUT​/api​/v1​/Authors​/{123567890123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/123567890123  
**Ожидаемый результат** Добавление списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 5f850922-7330-4891-84df-c172c43bcb54  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,
 "idBook": 0,
 "firstName": 
 "lastName": "string"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:48:15 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c0807c40d2354a49943f2d6c4b5a9f9c-a4a9d97e7ce66a4c-00",
    "errors": {
        "$": [
            "':' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 8 | BytePositionInLine: 11."
        ],
        "id": [
            "The value '123567890123' is not valid."
        ]
    }
}
```

#### 26.PUT​/api​/v1​/Authors​/{123567890123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/123567890123  
**Ожидаемый результат** Добавление списка авторов  
**Заголовки запроса**  

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 1d33f629-3dbf-4e0b-b2b9-8e287af5566a  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,
 "idBook": 0,
 "firstName": 555
 "lastName": "string"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 07:49:19 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-20b29e930ed1744fb1bd3144e186cc61-3455968430780f42-00",
    "errors": {
        "id": [
            "The value '123567890123' is not valid."
        ],
        "$.firstName": [
            "The JSON value could not be converted to System.String. Path: $.firstName | LineNumber: 6 | BytePositionInLine: 17."
        ]
    }
}
```

#### 27.DELETE ​/api​/v1​/Authors​/{123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/123  
**Ожидаемый результат** Удаление списка авторов  
**Заголовки запроса**  

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 5624f5f5-67df-436e-bbb1-4289cfffee43  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует

**Заголовки ответа**

Content-Length: 0  
Date: Fri, 09 Jun 2023 07:50:38 GMT  
Server: Kestrel  
api-supported-versions: 1.0  

**Тело ответа**отсутствует

### Books

#### 28. GET ​/api​/v1​/Books 

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Books  
**Ожидаемый результат** Получение списка книг  
**Заголовки запроса**  
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 37b1adda-171b-4dbf-ab5c-9e64573e3c79    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса** отсутствует 

**Заголовки ответа**     
Content-Type: application/json; charset=utf-8; v=1.0    
Date: Fri, 09 Jun 2023 08:26:23 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    
api-supported-versions: 1.0    

**Тело ответа**
```
[
    {
        "id": 1,
        "title": "Book 1",
        "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "pageCount": 100,
        "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "publishDate": "2023-06-08T08:32:14.562044+00:00"
    },
```

#### 29. POST ​/api​/v1​/Books

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books 

**Ожидаемый результат** Создание списка книг

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 429384ab-d10d-4a77-9cb9-ea0a903a680e    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 1,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:27:54.434Z"
}
```
**Заголовки ответа**     
Content-Type: application/json; charset=utf-8; v=1.0    
Date: Fri, 09 Jun 2023 08:38:43 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    
api-supported-versions: 1.0    

**Тело ответа**
```
{
  "id": 1,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:27:54.434Z"
}
```
#### 30. POST ​/api​/v1​/Books (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books  

**Ожидаемый результат** Создание списка книг

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: ddaccedc-d68b-40cf-af6c-838b980b5221    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": qwe,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:27:54.434Z"
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 08:42:37 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-54e7d941c1c40e43a3ab8f9673aa8522-b85ed9693525d640-00",
    "errors": {
        "$.id": [
            "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
        ]
    }
}
```

#### 31. POST ​/api​/v1​/Books (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books 

**Ожидаемый результат** Создание списка книг

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 4d8b3793-ff5e-4182-bcac-71cc7536e376    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "idd": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "20233-06-07T13:27:54.434Z"
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 08:46:30 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-227bdb3368956b44a67ec1fa7d57a1cb-e314b83c8c7c5a4e-00",
    "errors": {
        "$.publishDate": [
            "The JSON value could not be converted to System.DateTime. Path: $.publishDate | LineNumber: 6 | BytePositionInLine: 44."
        ]
    }
}
```

#### 32. POST ​/api​/v1​/Books (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books

**Ожидаемый результат** Создание списка книг

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 5adb0c08-dbc2-42cf-862b-721def59c29b    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": 
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 08:48:57 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-fb54642e02917347b44fc0444b566c00-9dc42cd40e708b4d-00",
    "errors": {
        "$.publishDate": [
            "'}' is an invalid start of a value. Path: $.publishDate | LineNumber: 7 | BytePositionInLine: 0."
        ]
    }
}
```

#### 33. POST ​/api​/v1​/Books (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books

**Ожидаемый результат** Создание списка книг

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 6c815c61-01c3-4f10-b666-f1f86bf332ef    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": 555
  "publishDate": 
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 08:52:11 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-35380a34d27d0e4188ac20c40eb203f6-ddae0d0abc06a744-00",
    "errors": {
        "$.excerpt": [
            "The JSON value could not be converted to System.String. Path: $.excerpt | LineNumber: 5 | BytePositionInLine: 16."
        ]
    }
}
```

#### 34. GET ​/api​/v1​/Books​/{1}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/1

**Ожидаемый результат** Получение книги под id=1

**Заголовки запроса**    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 13a0168c-6ea4-4af9-9c7c-ccb4c8eec81b    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  отсутствует

**Заголовки ответа**     
Content-Type: application/json; charset=utf-8; v=1.0    
Date: Fri, 09 Jun 2023 08:56:28 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    
api-supported-versions: 1.0    

**Тело ответа**
```
{
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-08T08:56:29.1170059+00:00"
}
```

#### 35. GET ​/api​/v1​/Books​/{11111111111} (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/11111111111  
**Ожидаемый результат** Получение книги под id=11111111111  

**Заголовки запроса**    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 2581a599-a577-40d5-82d1-5417a0089b62    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  отсутствует

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 09:07:59 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3cc2f73840dc8c4a87c58eba36144a2a-75adcc8a6d19a848-00",
    "errors": {
        "id": [
            "The value '11111111111' is not valid."
        ]
    }
}
```

#### 36. PUT ​/api​/v1​/Books​​/{1}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/1

**Ожидаемый результат** Добаление списка книг под id = 1

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: bded6487-7a0e-4b26-a038-c1864fafbb07    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:36:42.131Z"
}
```

**Заголовки ответа**     
Content-Type: application/json; charset=utf-8; v=1.0    
Date: Fri, 09 Jun 2023 09:09:11 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    
api-supported-versions: 1.0    

**Тело ответа**
```
{
    "id": 0,
    "title": "string",
    "description": "string",
    "pageCount": 0,
    "excerpt": "string",
    "publishDate": "2023-06-07T13:36:42.131Z"
}
```

#### 37. PUT ​/api​/v1​/Books​/{12345678901} (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/12345678901

**Ожидаемый результат** Добаление списка книг под id = 12345678901

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 068916e3-238c-4783-93b9-796c95cf7298    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:36:42.131Z"
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 09:14:10 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-d94c3efc8540894eaa76425fdef0b90a-6348631716fe7349-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}
```

#### 38. PUT ​/api​/v1​/Books​/{123} (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/123

**Ожидаемый результат** Добаление списка книг под id = 123

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: a98c2ddf-7536-4ef3-8c16-8b49ac6f0b99    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "idd": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "20233-06-07T13:36:42.131Z"
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 09:16:21 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-9a4247a80fee714d921071936f25d2f8-e57650694a63194c-00",
    "errors": {
        "$.publishDate": [
            "The JSON value could not be converted to System.DateTime. Path: $.publishDate | LineNumber: 6 | BytePositionInLine: 44."
        ]
    }
}
```

#### 39. PUT ​/api​/v1​/Books​/{123} (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/123

**Ожидаемый результат** Добаление списка книг под id = 123

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 2fa0ebda-e659-4f81-bb01-bd470ec56c90    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": 
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 09:45:55 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-8afc7740913b394e92083a918fc62415-a7389b07d8063443-00",
    "errors": {
        "$.publishDate": [
            "'}' is an invalid start of a value. Path: $.publishDate | LineNumber: 7 | BytePositionInLine: 0."
        ]
    }
}
```

#### 40. PUT ​/api​/v1​/Books​/{123} (провальный)

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/123

**Ожидаемый результат** Добаление списка книг под id = 123

**Заголовки запроса**    
Content-Type: application/json    
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: f8bdb2fa-67cc-497e-9996-c835d911a7fe    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  
```
{
  "id": 0,
  "title": "string",
  "description": 555
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-07T13:36:42.131Z"
}
```

**Заголовки ответа**     
Content-Type: application/problem+json; charset=utf-8    
Date: Fri, 09 Jun 2023 09:19:35 GMT    
Server: Kestrel    
Transfer-Encoding: chunked    

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-da4e528411eaa342b1cb95a4ea2ab776-1072f0fd69de824a-00",
    "errors": {
        "$.description": [
            "The JSON value could not be converted to System.String. Path: $.description | LineNumber: 3 | BytePositionInLine: 20."
        ]
    }
}
```

#### 41. DELETE ​/api​/v1​/Books​/{123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books/123

**Ожидаемый результат** Удаление списка книг под id = 123

**Заголовки запроса**        
User-Agent: PostmanRuntime/7.32.2    
Accept: */*    
Cache-Control: no-cache    
Postman-Token: 1185d65c-6c47-4ce8-b1cf-c28b4e972e70    
Host: fakerestapi.azurewebsites.net    
Accept-Encoding: gzip, deflate, br    
Connection: keep-alive    

**Тело запроса**  отсутствует

**Заголовки ответа**     
Content-Length: 0    
Date: Fri, 09 Jun 2023 09:25:49 GMT    
Server: Kestrel    
api-supported-versions: 1.0    

**Тело ответа** отсутствует

### CoverPhotos


#### 42.GET ​/api​/v1​/CoverPhotos  
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Получение фотограции  

**Заголовки запроса** 

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 4c69ada8-d2e3-4220-b1bc-c025f1544308  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  
**Заголовки ответа**  

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 12:10:29 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**

```
    {
        "id": 1,
        "idBook": 1,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
    },
    {
        "id": 2,
        "idBook": 2,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
    },
```

#### 43.POST ​/api​/v1​/CoverPhotos
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Отправка фотографии  

**Заголовки запроса**

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 7617a190-3d4f-4c7c-b8bb-b10a92b1434d  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 1,
 "idBook": 0,
 "url": "string"

}
```
**Заголовки ответа**

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 12:13:22 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
{
    "id": 1,
    "idBook": 0,
    "url": "string"
}
```

#### 44.POST ​/api​/v1​/CoverPhotos  
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Отправка фотографии  

**Заголовки запроса**   

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: ab5b02ba-79d1-4237-8b1c-411363f1cd6b  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": qwe,
 "idBook": 0,
 "url": "string"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:17:44 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-482b0b8f0ac89342ae304c0188adf651-a0b6763f1c99e341-00",
    "errors": {
        "$.id": [
            "'q' is an invalid start of a value. Path: $.id | LineNumber: 2 | BytePositionInLine: 7."
        ]
    }
}
```

#### 45.POST ​/api​/v1​/CoverPhotos  

**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Отправка фотографии  

**Заголовки запроса** 

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 141474b1-5a64-42ad-bf95-25cd374bb657  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "ida": 0,
 "idBook": 0,a
 "url": "strinag"

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:19:16 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-c0abd65c1591504c8f4b44ca7c7c45a3-0c1f9eb29ba1ba41-00",
    "errors": {
        "$": [
            "'a' is an invalid start of a property name. Expected a '\"'. Path: $ | LineNumber: 4 | BytePositionInLine: 13."
        ]
    }
}
```

#### 46.POST ​/api​/v1​/CoverPhotos

**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Отправка фотографии  

**Заголовки запроса** 

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 9e965209-b550-4e0e-bdc7-b9e28fbdf31a  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive    

**Тело запроса**
```
{

 "id": 0,

 "idBook": 0,

 "url": 

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:24:08 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-75549893e70d0b4e8f11ddf88d4a6ab3-64421b5c1271824e-00",
    "errors": {
        "$.url": [
            "'}' is an invalid start of a value. Path: $.url | LineNumber: 8 | BytePositionInLine: 0."
        ]
    }
}
```

#### 47.POST ​/api​/v1​/CoverPhotos

**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  
**Ожидаемый результат** Отправка фотографии  

**Заголовки запроса** 

Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 3d470e3a-4d72-4f09-89ff-587f10e7ac55  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**
```
{

 "id": 0,  
 "idBook": 0,  
 "url": 555  

}
```
**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:21:38 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-93d6251c09ab144f9af33a99688a485d-f6fa872069949344-00",
    "errors": {
        "$.url": [
            "The JSON value could not be converted to System.Uri. Path: $.url | LineNumber: 6 | BytePositionInLine: 11."
        ]
    }
}
```


#### 48.GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}  

**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/1  
**Ожидаемый результат** Получение фотографии  

**Заголовки запроса** 

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 286b32bd-fa41-4534-bc2e-dad3eb7974c0  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**

Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 12:27:46 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа**
```
[
    {
        "id": 1,
        "idBook": 1,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
    }
]
```

#### 49.GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}

**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/11111111111  
**Ожидаемый результат** Получение фотографии  
**Заголовки запроса**   

User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 58b96035-1c5e-457c-bb96-90aa22ca7ce7  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**

Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:29:39 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа**
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-fe6236d490f89e4cabb4cb7eeaad5aec-822571c9e8538c4c-00",
    "errors": {
        "idBook": [
            "The value '11111111111' is not valid."
        ]
    }
}
```

#### 50.GET/api/v1/CoverPhotos/{1}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1  

**Ожидаемый результат**   Получение фото id 1

**Заголовки запроса **                    
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: a7bca49c-64b9-465e-ba4a-78a2016f1887  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**                        
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 12:11:46 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа** 

```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
}
```

#### 51.GET/api/v1/CoverPhotos/{12345678901}

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/12345678901  

**Ожидаемый результат**   Получение из списка юзера id12345678901  

**Заголовки запроса **                  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 94f2c28f-f4db-435a-89d9-fba3472e40b8  

Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:15:57 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-647cf1568b2c184eb55df31050fcb9f2-1a62e71ff0baec4b-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}

```

#### 52.PUT/api/v1/CoverPhotos/{1} 

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1  

**Ожидаемый результат**   Добавление фото 1

**Заголовки запроса **                    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 60d53f4f-5779-4a0c-bb22-c23f52548c36  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса**  

```
{
 "id": 0,
 "idBook": 0,
 "url": "string"
}
```

**Заголовки ответа**                        
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 12:19:22 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
**Тело ответа** 

```
{
    "id": 0,
    "idBook": 0,
    "url": "string"
}
```


#### 53.PUT/api/v1/CoverPhotos/{1234567890123} 

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1234567890123

**Ожидаемый результат**  Добавление фото  id234567890123

**Заголовки запроса **                  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 7ddfb950-f881-43a6-a45c-ed2fea501fed  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "idBook": 0,
 "url": "string"
}
```

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:23:07 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-ce74ff26e4e0a24cbc608484f3e8c21b-991388ebf5f7954b-00",
    "errors": {
        "id": [
            "The value '1234567890123' is not valid."
        ]
    }
}
```

#### 54.PUT/api/v1/CoverPhotos/{123} 

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123  

**Ожидаемый результат**   Добавление фото id123

**Заголовки запроса ** 
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 40465f0e-04c2-424c-b3fd-71030edc3772  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id"d: 0,
 "idBook": 0,
 "url": "stringgg"
}
```

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:25:57 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3b3b97d8afa5544496192253b9bbf14d-50b4d6417cfc4d46-00",
    "errors": {
        "$": [
            "'d' is invalid after a property name. Expected a ':'. Path: $ | LineNumber: 2 | BytePositionInLine: 5."
        ]
    }
}
```



#### 55.PUT/api/v1/CoverPhotos/{123} 

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123

**Ожидаемый результат**   Добавление фото id123  

**Заголовки запроса **                  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 65c5b7f4-0a19-4773-a39f-b8b00628dbc3  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "id": 0,
 "idBook": 0,
 "url": 
}
```

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:40:30 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3d9d446bbeba9d4dba3c767d4a96c210-390e4b6741dea54a-00",
    "errors": {
        "$.url": [
            "'}' is an invalid start of a value. Path: $.url | LineNumber: 5 | BytePositionInLine: 0."
        ]
    }
}
```

#### 56.PUT/api/v1/CoverPhotos/{123} 

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123

**Ожидаемый результат**  Добавление фото  id123 

**Заголовки запроса **                  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 0f26d618-09da-47f5-b470-2c674c9c3e8e  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 
```
{
 "id": 0,
 "idBook": 0,
 "url": 555
}
```

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 12:43:26 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-f6b0fd1177a2be47b0c779dea260b069-b9e49be7b5e93c42-00",
    "errors": {
        "$.url": [
            "The JSON value could not be converted to System.Uri. Path: $.url | LineNumber: 6 | BytePositionInLine: 11."
        ]
    }
}
```

### 57.DELETE/api/v1/CoverPhotos/{123}

**URL ** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123  

**Ожидаемый результат**   Удаление из списка фото id123

**Заголовки запроса **                  
User-Agent: PostmanRuntime/7.32.2  
Accept: */  *
Cache-Control: no-cache  
Postman-Token: 2a08f9e3-cad7-4e05-ab07-6c9fffa201f6  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**                        

Content-Length: 0  
Date: Fri, 09 Jun 2023 12:45:46 GMT  
Server: Kestrel  
api-supported-versions: 1.0  
**Тело ответа** отсутствует  

## Users

### 58.GET/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users

**Ожидаемый результат**  Получение списка юзеров  

**Заголовки запроса ** 
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 005cffdf-a350-4b8e-ad1e-ec868514c838  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**  
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 09:00:24 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа** 

```
[
    {
        "id": 1,
        "userName": "User 1",
        "password": "Password1"
    },
    {
        "id": 2,
        "userName": "User 2",
        "password": "Password2"
    },
    
```


### 59.POST/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users  

**Ожидаемый результат**  Отправка списка юзеров    

**Заголовки запроса **   
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */  *
Cache-Control: no-cache  
Postman-Token: 92f0885d-a418-4af9-af96-732aa20824e1  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
    "id": 0,
    "userName": "string",
    "password": "string"
}
```

**Заголовки ответа**  
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 09:13:00 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "id": 0,
    "userName": "string",
    "password": "string"
}
```

### 60.POST/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users  

**Ожидаемый результат**  Отправка списка юзеров      

**Заголовки запроса **     
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: a30ca0c2-42e8-42c9-953b-4315cb9e1edd  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
   {
 "id": qwe,
 "title": "string",
 "description": "string",
 "pageCount": 0,
 "excerpt": "string",
 "publishDate": "2023-06-06T10:23:21.642Z"
}
```

**Заголовки ответа**    
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:17:44 GMT  
Server: Kestrel  
Transfer-Encoding: chunked   

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-48094e98455f424cb8d3d92c24791411-1a972f9931cb674e-00",
    "errors": {
        "$.id": [
            "'q' is an invalid start of a value. Path: $.id | LineNumber: 2 | BytePositionInLine: 7."
        ]
    }
}
```

### 61.POST/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users

**Ожидаемый результат**  Отправка списка юзеров      

**Заголовки запроса **    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: f3d1436b-749c-44fa-abbf-ad314f50feb3  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive     

**Тело запроса** 

```
 {
 "idd": w0,
 "userNamee": "string",
 "password": "striing"
}
```
**Заголовки ответа**      
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:21:52 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-bcd2c0b963a64e4fb03c8b350c5bf83a-8b4085e0f5bb0744-00",
    "errors": {
        "$.idd": [
            "'w' is an invalid start of a value. Path: $.idd | LineNumber: 2 | BytePositionInLine: 8."
        ]
    }
}
```


### 62.POST/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users

**Ожидаемый результат**  Отправка списка юзеров      

**Заголовки запроса **      
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */* 
Cache-Control: no-cache  
Postman-Token: 15a6056b-6fe4-47aa-a217-59dbe96fcd80  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
 {
 "id": 0,
 "userName":
 "password": "string"
}
```

**Заголовки ответа**        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:24:56 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-67e0b1e4c674b44fa896cf1fb5c7a11b-a71840e7e80d1f42-00",
    "errors": {
        "$": [
            "':' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 6 | BytePositionInLine: 11."
        ]
    }
}
```

### 63.POST/api/v1/Users

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users

**Ожидаемый результат**  Отправка списка юзеров      

**Заголовки запроса**        
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: cb5d90dc-f9c1-4ea1-a425-7c29b253c221  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "userName": 555
 "password": "string"
}
```

**Заголовки ответа**          
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:27:27 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
    {
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-53e88ddb8ecfec428220ce9f8d2e4383-2af22f05982bd341-00",
    "errors": {
        "$.userName": [
            "The JSON value could not be converted to System.String. Path: $.userName | LineNumber: 4 | BytePositionInLine: 16."
        ]
    }
}
```

### 64.GET/api/v1/Users/{1}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users/1

**Ожидаемый результат**   Получение из списка юзера id1    

**Заголовки запроса**          
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: b610cf98-3fce-4f9c-a6a0-4eca2d33aa82  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** Отсутствует

**Заголовки ответа**            
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 09:30:42 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0  

**Тело ответа** 

```
{
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
}
```

### 65.GET/api/v1/Users/{11111111111}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/11111111111

**Ожидаемый результат**   Получение из списка юзера id11111111111     

**Заголовки запроса**            
User-Agent: PostmanRuntime/7.32.2  
Accept: */  *
Cache-Control: no-cache  
Postman-Token: 789e6080-2c1c-4afe-9e57-503965507692  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br 
Connection: keep-alive  
**Тело запроса** Отсутствует  
**Заголовки ответа**                
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:36:32 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-748039426d9af644bc077f421baf4624-2919aabf33e2b34a-00",
    "errors": {
        "id": [
            "The value '11111111111' is not valid."
        ]
    }
}
```

### 66.PUT/api/v1/Users/

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/1

**Ожидаемый результат**   Получение из списка юзера id1   

**Заголовки запроса**              
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 74be0c3c-dcd0-488b-90b5-6c069e3a2fb0  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "userName": "string",
 "password": "string"
}
```

**Заголовки ответа**                  
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Fri, 09 Jun 2023 09:39:14 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0   

**Тело ответа** 

```
{
    "id": 0,
    "userName": "string",
    "password": "string"
}
```


### 67.PUT/api/v1/Users/{12345678901}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/12345678901

**Ожидаемый результат**   Получение из списка юзера id12345678901 

**Заголовки запроса**                
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 94246d1b-1121-42de-988c-a963e6f63789  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "userName": "string",
 "password": "string"
}
```

**Заголовки ответа**                    
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:42:34 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-cd1c37472d9e154d8dccc8cb068844e9-46e39c01c7c4fb42-00",
    "errors": {
        "id": [
            "The value '12345678901' is not valid."
        ]
    }
}
```

### 68.PUT/api/v1/Users/{123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/123

**Ожидаемый результат**   Получение из списка юзера id123

**Заголовки запроса**                  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: faa96dcc-8101-4cac-b51d-697229f2db4a  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": d0,
 "userName": "string",
 "password": "string"
}
```

**Заголовки ответа**                      
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:45:32 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-38087a243df299438975c698c0e69b49-35f191360861694d-00",
    "errors": {
        "$.id": [
            "'d' is an invalid start of a value. Path: $.id | LineNumber: 2 | BytePositionInLine: 7."
        ]
    }
}
```


### 69.PUT/api/v1/Users/{123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/123  

**Ожидаемый результат**   Получение из списка юзера id 123  

**Заголовки запроса**                    
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: efab83a3-48c9-4ee6-a0a2-7e79f292f637  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "userName": 
 "password": "string"
}
```
**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:48:28 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-166d0a467b33f14fb9267588336f2b71-4696daad3bf28a43-00",
    "errors": {
        "$": [
            "':' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 6 | BytePositionInLine: 11."
        ]
    }
}
```

### 70.PUT/api/v1/Users/{123}

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/123

**Ожидаемый результат**   Получение из списка юзера id123

**Заголовки запроса**                  
Content-Type: application/json  
User-Agent: PostmanRuntime/7.32.2  
Accept: */ * 
Cache-Control: no-cache  
Postman-Token: 1ef74977-8716-4e51-93a6-c795e999e625  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** 

```
{
 "id": 0,
 "userName": 555
 "password": "string"
}
```

**Заголовки ответа**                        
Content-Type: application/problem+json; charset=utf-8  
Date: Fri, 09 Jun 2023 09:52:00 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  

**Тело ответа** 

```
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-facc8fa13689a34695d6bcd06111a94f-720547ef1f804f45-00",
    "errors": {
        "$.userName": [
            "The JSON value could not be converted to System.String. Path: $.userName | LineNumber: 4 | BytePositionInLine: 16."
        ]
    }
}
```

### 71.DELETE/api/v1/Users/{123}

**URL**  https://fakerestapi.azurewebsites.net/api/v1/Users/123

**Ожидаемый результат**   Удаление из списка юзера id123

**Заголовки запроса**                  
User-Agent: PostmanRuntime/7.32.2  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: b2fd97ee-0fb1-47a5-affa-10b676c1bf53  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive  

**Тело запроса** отсутствует  

**Заголовки ответа**                       
Content-Length: 0  
Date: Fri, 09 Jun 2023 09:53:46 GMT  
Server: Kestrel  
api-supported-versions: 1.0  

**Тело ответа** отсутствует    
