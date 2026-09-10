### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

url:localhost:5000/movies/  
method:post  
body{  
    title:"kgf1",  
    year :2008,  
    language:"kannada",  
    run_time=160  
}

`http_request for list all movie`  
url:localhost:5000/movies/  
method:list  

`http_request for fetching movie detail`  
url:localhost:5000/movies/2/  
method:get  

`http_request for update movie`  
url:localhost:5000/movies/2/    
method:put  
body{  
    title:Jhon wick  
    year:2020  
    language:Engilsh  
    run_time:160  
    
}  
`http_request for delete movie`  
url(localhost:5000/movies/2)  
method:delete  

--Hospital
patient_id    patient_name  phone_number   assigned_doctor   department    appointment_date   status     fees  

     1           Jhon        9302948593       Dr.Alex         Fitness         12.03.2026      Pending     230  
     2           Adham       8557553243       Dr.lallu        Ortho           13.03.2026      Complete    250 
     3           Reena       8721038497       Dr.Sheena       Skin            14.03.2026      Processing  250 
    

`http_request for adding new patients`  
url(lacalhost:1500/patients/)  
method:Post  
body{  
    patient_name:Ahemmad  
    phone_number:8913986532    
    assigned_doctor:Dr Thankachan   
    department:Cardio  
    appointment_date:14.04.2026  
    status:Complete  
    fees:260  
}

`http_request for list all patients`  
url(localhost:1500/patients/)  
method:Get  

`http_request for fetching patients detail`  
uel(localhost:1500/patients/3/)  
method:Get  

`http_request for update pateints`  
url(localhost:1500/patients/2/)  
method:Patch(  

    assigned_doctor:Dr Devichan  
    department:Deititian  
)

`http_request for delete pateints`

url(localhost:1500/patients/4/)  
method:Delete  

