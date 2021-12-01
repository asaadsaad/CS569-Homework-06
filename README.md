# CS569 Homework 06
## Dependency Injection Framework
### Coding Exercise
* Update the global CSS styles with the following code:
```css
body {
	display: flex;
}
```
* Create a service that has a method `getData()` that sends an HTTP request to the following URL:
```js
https://randomuser.me/api/?results=10
```
* The application should call `getData()` at bootstrap time, and save the response into the `localStorage`. 
* Add another method to your service `getCachedData()` that returns an observable with a JSON object reads from `localStorage`.
* Create a button on your root component to Show/Hide `UsersComponent`. 
* `UsersComponent` will simply call the `getCachedData()` method and display list of users, each user should be displayed using a reusable component called: `UserComponent`. 
* The `UserComponent` will only display the first/last name, date of birth, full address, and phone number of the user. Each user should be displayed as a card, use the following CSS formatting:
```css
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
  margin: 10px;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}
```
A card has the following HTML structure:
```html
<div class="card">
  <div class="container">
    <h4>Asaad Saad</h4>
    <p>Dec 1st, 2020</p>
    <p>1000 N 4th Street, Fairfield, IA 52557</p>
    <p>+19998881111</p>
  </div>
</div>
```
* Use pipes to format the date of birth and phone numbers to start with `+1` and remove all hyphen symbols..

