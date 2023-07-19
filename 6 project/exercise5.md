**Activities**

 **1. GET/api/v1/Activities**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Activities
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-01T13:25:47.5012071+00:00",
    "completed": false
  },
   {
    "id": 2,
    "title": "Activity 2",
    "dueDate": "2023-06-01T14:25:47.5012094+00:00",
    "completed": true
  },
  {
    "id": 3,
    "title": "Activity 3",
    "dueDate": "2023-06-01T15:25:47.5012097+00:00",
    "completed": false
```

**2. POST /api​/v1​/Activities - успешный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Activities
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 1,
  "title": "string",
  "dueDate": "2023-06-02T06:15:30.563Z",
  "completed": true
}
```
5. 200
6. 
```
{
  "id": 1,
  "title": "string",
  "dueDate": "2023-06-02T06:15:30.563Z",
  "completed": true
}
```

**3. POST​/api​/v1​/Activities - провальный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Activities
3. accept: text/plain; v=1.0
4. 
```
{
  "id": sdfsdf,
  "title": "string",
  "dueDate": "2023-06-02T06:15:30.563Z",
  "completed": true
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-938d6c59e2c86a459fea2a75178eb959-594b5bd0c245094c-00",
  "errors": {
    "$.id": [
      "'s' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**4. GET ​/api​/v1​/Activities​/{id} -успешный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Activities/1
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
{
  "id": 1,
  "title": "Activity 1",
  "dueDate": "2023-06-02T14:17:07.9882822+00:00",
  "completed": false
}
```

**5. GET ​/api​/v1​/Activities​/{id} -провальный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Activities/69
3. accept: text/plain; v=1.0
4. отсутствует
5. 404
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-1ef16ea42e43b0479fe095a37e06d7c0-6b18622ef8fc9645-00"
}
```
**6. PUT ​/api​/v1​/Activities​/{id} - успешный**

1. PUT 
2. https://fakerestapi.azurewebsites.net/api/v1/Activities/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 123,
  "title": "string",
  "dueDate": "2023-06-02T06:19:33.684Z",
  "completed": true
}
```
5. 200
6. 
```
{
  "id": 123,
  "title": "string",
  "dueDate": "2023-06-02T06:19:33.684Z",
  "completed": true
}
```
**7. PUT ​/api​/v1​/Activities​/{id} - провальный**

1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Activities/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": qwe,
  "title": "string",
  "dueDate": "2023-06-02T06:19:33.684Z",
  "completed": true
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c07a5929c0a20043bbd270013f798260-a821d5e72c70f541-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**8.DELETE ​/api​/v1​/Activities​/{id} - успешный**

1. DELETE
2. https://fakerestapi.azurewebsites.net/api/v1/Activities/1234567890
3. accept: ```*/*```
4. отсутствует
5. 200
6. отсутствует

**9. GET ​/api​/v1​/Authors**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Authors
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
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
  {
    "id": 3,
    "idBook": 1,
    "firstName": "First Name 3",
    "lastName": "Last Name 3"
  },
```
**10. POST ​/api​/v1​/Authors - успешный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Authors
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 123,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. 200
6. 
```
{
  "id": 123,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
**11. POST ​/api​/v1​/Authors - провальный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Authors
3. accept: text/plain; v=1.0
4. 
```
{
  "id": qwe,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-8895f4a4923a3f4b8b51ebde4de0682e-dee7363248ba1445-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**12. GET ​/api​/v1​/Authors​/authors​/books​/{idBook} - успешный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/1
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
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
**13. GET ​/api​/v1​/Authors​/authors​/books​/{idBook} - провальный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/12345678901
3. accept: text/plain; v=1.0
4. отсутствует
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-0a5e574b97429c43aa732a767113e55a-8792bf54e943f749-00",
  "errors": {
    "idBook": [
      "The value '12345678901' is not valid."
    ]
  }
}
```
**14. GET ​/api​/v1​/Authors​/{id} - успешный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/123
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
{
  "id": 123,
  "idBook": 41,
  "firstName": "First Name 123",
  "lastName": "Last Name 123"
}
```
**15. GET ​/api​/v1​/Authors​/{id} - провальный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/1234567890
3. accept: text/plain; v=1.0
4. отсутствует
5. 404
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-5171a8ade1ecfe439cf03820572edfb6-0bd340a985632543-00"
  }
```
**16. PUT ​/api​/v1​/Authors​/{id} - успешный**

1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 1,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. 200
6. 
```
{
  "id": 1,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

**17. PUT ​/api​/v1​/Authors​/{id} - провальный**

1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": qwe,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b3ac78a6e1b8244287bba4be1092f1c6-69070795baa0e94b-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```

**18. DELETE ​/api​/v1​/Authors​/{id} - успешный**

1. DELETE
2. https://fakerestapi.azurewebsites.net/api/v1/Authors/123
3. accept: ```*/*```
4. отсутствует
5. 200
6. отсутствует

**BOOKS**

**19. GET ​/api​/v1​/Books - успешный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Books
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
  {
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-01T18:32:15.8319766+00:00"
  },
  {
    "id": 2,
    "title": "Book 2",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 200,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-05-31T18:32:15.8319907+00:00"
  },
```

**20. POST ​/api​/v1​/Books - успешный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Books
3. accept: ```*/*```
4. 
```
{
  "id": 123,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T18:35:22.976Z"
}
```
5. 200
6. 
```
{
  "id": 123,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T18:35:22.976Z"
}
```
**21. POST ​/api​/v1​/Books - провальный**

1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Books
3. accept: ```*/*```
4. 
```
{
  "id": qwe,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T18:35:22.976Z"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3352e936164bbd4c94ce0e492e500b43-eb0f7b354e306c4f-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```

**22. GET ​/api​/v1​/Books​/{id} -успешный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Books/123
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
{
  "id": 123,
  "title": "Book 123",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 12300,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-01-30T18:43:54.3350473+00:00"
}
```

**23. GET ​/api​/v1​/Books​/{id} -провальный**

1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Books/1234
3. accept: text/plain; v=1.0
4. отсутствует
5. 404
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-28c56ce166651547825bc397b18fc565-d8551d4ad648d445-00"
}
```
**24. PUT ​/api​/v1​/Books​/{id} - успешный**

1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Books/123
3. accept: ```*/*```
4.
```
{
  "id": 123,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T20:20:03.099Z"
}
```
5. 200
6. 
```
{
  "id": 123,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T20:20:03.099Z"
}
```
**25. PUT ​/api​/v1​/Books​/{id} - провальный**
1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Books/123
3. accept: ```*/*```
4. 
```
{
  "id": qwe,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-02T20:20:03.099Z"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-3218e1dfb77030489e316002b4ab4f82-ae9846fc9a9e7c44-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**26.DELETE ​/api​/v1​/Books​/{id} - успешный**
1. DELETE
2. https://fakerestapi.azurewebsites.net/api/v1/Books/123
3. ```accept: */*```
4. отсутствует
5. 200
6. отсутствует

**CoverPhotos**

**27. GET ​/api​/v1​/CoverPhotos - успешный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
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
  {
    "id": 3,
    "idBook": 3,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 3&w=250&h=350"
  },
```
**28. POST ​/api​/v1​/CoverPhotos - успешный**
1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 123,
  "idBook": 0,
  "url": "string"
}
```
5. 200
6. 
```
{
  "id": 123,
  "idBook": 0,
  "url": "string"
}
```
**29. POST ​/api​/v1​/CoverPhotos - провальный**
1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. accept: text/plain; v=1.0
4. 
```
{
  "id": qwe,
  "idBook": 0,
  "url": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-ecf04c1c178ceb49963ecd9e18c82db2-de7d637c967cd743-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**30. GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook} - успешный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/123
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
[
  {
    "id": 123,
    "idBook": 123,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 123&w=250&h=350"
  }
]
```
**31. GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook} - провальный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/12345678901
3. accept: text/plain; v=1.0
4. отсутствует
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-8817cadf602a1f4a987ccf9750074799-8f83ab77a7615248-00",
  "errors": {
    "idBook": [
      "The value '12345678901' is not valid."
    ]
  }
}
```
**32. GET ​/api​/v1​/CoverPhotos​/{id} - успешный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
```
{
  "id": 123,
  "idBook": 123,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 123&w=250&h=350"
}
```
**33. GET ​/api​/v1​/CoverPhotos​/{id} - провальный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/12345678901
3. accept: text/plain; v=1.0
4. отсутствует
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-8699593a43f5694f8faebbd4cc35832d-24f6e07f3a0b4845-00",
  "errors": {
    "id": [
      "The value '12345678901' is not valid."
    ]
  }
}
```
**34. PUT ​/api​/v1​/CoverPhotos​/{id} - успешный**
1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": 123,
  "idBook": 0,
  "url": "string"
}
```
5. 200
6. 
```
{
  "id": 123,
  "idBook": 0,
  "url": "string"
}
```
**35. PUT ​/api​/v1​/CoverPhotos​/{id} - провальный**
1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123
3. accept: text/plain; v=1.0
4. 
```
{
  "id": qwe,
  "idBook": 0,
  "url": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e5b7d7afddc3f04b9683642569d4b0af-0d5865ea63197447-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**36. DELETE ​/api​/v1​/CoverPhotos​/{id} - успешный**
1. DELETE
2. https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123
3. accept: ```*/*```
4. отсутствует
5. 200
6. отсутствует

**USER**

**37. GET /api​/v1​/Users**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Users
3. accept: text/plain; v=1.0
4. отсутствует
5. 200
6. 
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
  {
    "id": 3,
    "userName": "User 3",
    "password": "Password3"
  },
```
**38. POST ​/api​/v1​/Users - успешный**
1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Users
3. accept: ```*/*```
4. 
```
{
  "id": 123,
  "userName": "string",
  "password": "string"
}
```
5. 200
6. 
```
{
  "id": 123,
  "userName": "string",
  "password": "string"
}
```
**39. POST ​/api​/v1​/Users - провальный**
1. POST
2. https://fakerestapi.azurewebsites.net/api/v1/Users
3. accept: ```*/*```
4. 
```
{
  "id": qwe,
  "userName": "string",
  "password": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-13dcf1c4500f9743b34b3dc6f6fd76cd-469afa34c9f2ac4c-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**40. GET ​/api​/v1​/Users​/{id} -успешный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Users/1
3. accept: ```*/*```
4. отсутствует
5. 200
6. 
```
{
  "id": 1,
  "userName": "User 1",
  "password": "Password1"
}
```
**41. GET ​/api​/v1​/Users​/{id} -провальный**
1. GET
2. https://fakerestapi.azurewebsites.net/api/v1/Users/123
3. accept: ```*/*```
4. отсутствует
5. 404
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-d4f44748ee8b924fac3ea297968bcff6-f56200dd16201544-00"
}
```
**42. PUT ​/api​/v1​/Users​/{id} - успешный**
1. PUT
2. https://fakerestapi.azurewebsites.net/api/v1/Users/123
3. accept: ```*/*```
4. 
```
{
  "id": 123,
  "userName": "string",
  "password": "string"
}
```
5. 200
6. 
```
{
  "id": 123,
  "userName": "string",
  "password": "string"
}
```
**43. PUT ​/api​/v1​/Users​/{id} - провальный**
1. PUT 
2. https://fakerestapi.azurewebsites.net/api/v1/Users/123
3. accept: ```*/*```
4. 
```
{
  "id": qwe,
  "userName": "string",
  "password": "string"
}
```
5. 400
6. 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-d1324c032a33d14c8360ddc55da767fd-a5ce896d21ac8843-00",
  "errors": {
    "$.id": [
      "'q' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
**44. DELETE ​/api​/v1​/Users​/{id} - успешный**
1. DELETE
2. https://fakerestapi.azurewebsites.net/api/v1/Users/123
3. accept: ```*/*```
4. отсутствует
5. 200
6. отсутствует
