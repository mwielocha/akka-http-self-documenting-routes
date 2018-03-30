# ExampleApi

* [ExampleApi](#exampleapi)

    *  [POST /api/image](#post-apiimage)  
    *  [GET /api/user](#get-apiuser)  
    *  [POST /api/user](#post-apiuser)  
    *  [PUT /api/users](#put-apiusers)  
    *  [GET /api/users](#get-apiusers)  
    *  [GET /api/users/{integer}](#get-apiusersinteger)  



##  [POST /api/image](#post-apiimage) 
(multipart/form-data; boundary=b7nKPzJpa0Do+YuCSNnFspJt)





### Request body

**data:**

(application/json)
```json
{
   "image" : 100
}
```
**attachment:**

(application/octet-stream)
```
[application/octet-stream]
```




### Response 200
(application/json)

```json
"multipart/form-data"
```


##  [GET /api/user](#get-apiuser) 
(none/none)

 Fetch user 


### URL Parameters
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
  name | false | string |  | Just some user name | John 


### Request body


(none/none)
```
[none/none]
```




### Response 200
(application/json)

```json
{
   "id" : 1,
   "name" : "Jim"
}
```


##  [POST /api/user](#post-apiuser) 
(application/json)

 Fetch user 



### Request body


```json
{
   "id" : 2,
   "name" : "Hello"
}
```




### Response 200
(application/json)

```json
{
   "id" : 2,
   "name" : "Hello"
}
```


##  [PUT /api/users](#put-apiusers) 
(none/none)





### Request body


(none/none)
```
[none/none]
```




### Response 405
(text/plain; charset=UTF-8)

```
HTTP method not allowed, supported methods: GET
```


##  [GET /api/users](#get-apiusers) 
(none/none)




### URL Parameters
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
  offset |  | number |  |  | 0 
  limit |  | number |  |  | 10 


### Request body


(none/none)
```
[none/none]
```



### Request headers
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
  Authorization |  | string |  |  | Basic YWRtaW46YWRtaW4= 


### Response 200
(application/json)

```json
[
   {
      "id" : 1,
      "name" : "John"
   },
   {
      "id" : 2,
      "name" : "Jim"
   },
   {
      "id" : 3,
      "name" : "Jake"
   },
   {
      "id" : 4,
      "name" : "Jacob"
   },
   {
      "id" : 5,
      "name" : "Jane"
   }
]
```


##  [GET /api/users/{integer}](#get-apiusersinteger) 
(none/none)





### Request body


(none/none)
```
[none/none]
```




### Response 200
(application/json)

```json
{
   "id" : 3,
   "name" : "Jake"
}
```