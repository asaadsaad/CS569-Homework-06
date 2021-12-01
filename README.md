# CS569 Homework 06
## Dependency Injection Framework
### Coding Exercise
* Create a service that has a method `getData()` that sends an HTTP request to the following URL:
```js
https://randomuser.me/api/?results=10
```
* The application should call `getData()` at bootstrap time, and save the response into the `localStorage`. 
* Add another method to your service `getCachedData()` that returns an observable with a JSON object reads from `localStorage`.
* Create a button on your root component to Show/Hide `UsersComponent`. 
* `UsersComponent` will simply call the `getCachedData()` method and display list of users, each user should be displayed using a reusable component called: `UserComponent`. 
* The `UserComponent` will only display the first/last name, date of birth, full address, and phone number of the user.
* Use pipes to format the date of birth and phone numbers to start with `+1` and remove all hyphen symbols..

