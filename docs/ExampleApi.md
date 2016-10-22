# ExampleApi

* [ExampleApi](#exampleapi)

    *  [GET /api/user](#get-apiuser)  
    *  [POST /api/user](#post-apiuser)  
    *  [POST /api/user](#post-apiuser)  
    *  [GET /api/users](#get-apiusers)  
    *  [GET /api/users/{index}](#get-apiusers{index})  
    *  [GET /api/users/{index}](#get-apiusers{index})  



##  [GET /api/user](#get-apiuser) 
(none/none)


### URL Parameters
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
 name | | string | | | John
    


### Request body

no content



### Response 200
(application/json)

```json
{
  "id": 1,
  "name": "Jim"
}
```


##  [POST /api/user](#post-apiuser) 
(application/json)



### Request body

```json
{
  "id": 2,
  "name": "Hello"
}
```



### Response 200
(application/json)

```json
{
  "id": 2,
  "name": "Hello"
}
```


##  [POST /api/user](#post-apiuser) 
(application/json)



### Request body

```json
{
  "id": 500,
  "name": "Jimbo"
}
```



### Response 200
(application/json)

```json
{
  "id": 500,
  "name": "Jimbo"
}
```


##  [GET /api/users](#get-apiusers) 
(none/none)


### URL Parameters
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
 offset | | number | | | 0
     limit | | number | | | 10
    


### Request body

no content


### Request headers
Name        | required | type     | default value | description | example value
--- | ---  | --- | --- | --- | ---
 Authorization | | string | | | Basic YWRtaW46YWRtaW4=
    


### Response 200
(application/json)

```json
[{
  "id": 1,
  "name": "John"
}, {
  "id": 2,
  "name": "Jim"
}, {
  "id": 3,
  "name": "Jake"
}, {
  "id": 4,
  "name": "Jacob"
}, {
  "id": 5,
  "name": "Jane"
}]
```


##  [GET /api/users/{index}](#get-apiusers{index}) 
(none/none)



### Request body

no content



### Response 200
(application/json)

```json
{
  "id": 3,
  "name": "Jake"
}
```


##  [GET /api/users/{index}](#get-apiusers{index}) 
(none/none)



### Request body

no content



### Response 200
(application/json)

```json
{
  "id": 4,
  "name": "Jacob"
}
```
