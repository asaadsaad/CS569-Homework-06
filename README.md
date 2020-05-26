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
            "title":"Mr",
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
            "timezone":{
               "offset":"+6:00",
               "description":"Almaty, Dhaka, Colombo"
            }
         },
         "email":"ricky.grant@example.com",
         "login":{
            "uuid":"c5c2ba05-ddad-420d-b9b8-c5d4658e4cca",
            "username":"redleopard823",
            "password":"marc",
            "salt":"Z1O2ja1p",
            "md5":"ecc9aada12674ad1f37267291db1abcd",
            "sha1":"da94d13c9bf5b2d171405ac3d0ad7a3ad8e53ace",
            "sha256":"3c2edf25faadd91425a4cc9c68de081ed95efd24bb516b8f45d27c92284d6e99"
         },
         "dob":{
            "date":"1961-11-14T03:17:43.329Z",
            "age":59
         },
         "registered":{
            "date":"2017-05-09T07:14:56.450Z",
            "age":3
         },
         "phone":"(335)-827-7611",
         "cell":"(411)-558-2011",
         "id":{
            "name":"SSN",
            "value":"061-03-4082"
         },
         "picture":{
            "large":"https://randomuser.me/api/portraits/men/29.jpg",
            "medium":"https://randomuser.me/api/portraits/med/men/29.jpg",
            "thumbnail":"https://randomuser.me/api/portraits/thumb/men/29.jpg"
         },
         "nat":"US"
      }
   ],
   "info":{
      "seed":"e86dea4bfc637e06",
      "results":1,
      "page":1,
      "version":"1.3"
   }
}
```
* The application should call `getData()`, stringify the returned value, and save it into the `localStorage`. 
* The service has another method `getCachedData()` that returns an observable with a JSON object reads from `localStorage`.


