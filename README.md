# CS569 Homework 
### Coding Exercise
In a new Angular application, create the following:  
  
  * User service `user.service.ts`
  * Users container component `users.component.ts` (stateful)
  * User card representational component `user.component.ts` (stateless)
  
Implementation details:  
1. Create a button on your root component to Show/Hide (Mount/Unmount) the `UsersComponent` which is hidden by default. 
2. Your service has a method `getData()` that sends a GET request to the following URL:
```js
https://randomuser.me/api/?results=10
```
Make sure you set the response type(s), you may use [JSON to TypeScript service](https://transform.tools/json-to-typescript)
  
3. `UsersComponent` will call the `getData()` method and display list of users (try subscribe and async pipe), each user should be displayed using `UserComponent`. 
4. The the `UserComponent` will display the user picture, first/last name, date of birth, full address, and phone number of the user. Each user should be displayed as a card, you may use the following [Card Template](https://www.w3schools.com/howto/howto_css_cards.asp).

5. Use pipes to format the date of birth, and phone numbers to start with `+1`..

