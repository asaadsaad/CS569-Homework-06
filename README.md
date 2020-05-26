# CS569 Homework 07
## Dependency Injection Framework
### Coding Exercise
* Create a service that has a method `getData()` that returns the following JSON object:
```json
{
   "results":[
      {
         "gender":"male",
         "name":{
            "first":"Ricky",
            "last":"Grant"
         },
         "location":{
            "street":{
               "number":1681,
               "name":"Ranchview Dr"
            },
            "city":"Oklahoma City",
            "state":"Alabama",
            "country":"United States",
            "postcode":43719,
            "coordinates":{
               "latitude":"80.3503",
               "longitude":"-75.9276"
            },
         },
         "email":"ricky.grant@example.com",
         "dob":{
            "date":"1961-11-14T03:17:43.329Z",
            "age":59
         },
         "phone":"(335)-827-7611",
         "cell":"(411)-558-2011",
         "picture":{
            "large":"https://randomuser.me/api/portraits/men/29.jpg",
            "medium":"https://randomuser.me/api/portraits/med/men/29.jpg",
            "thumbnail":"https://randomuser.me/api/portraits/thumb/men/29.jpg"
         },
         "nat":"US"
      }
   ],
}
```
* The application should call `getData()` at bootstrap time, stringify the returned value, and save it into the `localStorage`. 
* The service has another method `getCachedData()` that returns an observable with a JSON object reads from `localStorage`.
* Create a custom component to display the user details using `getCachedData()` method, use pipes to format the date of birth properly and phone numbers to start with `+1`.


