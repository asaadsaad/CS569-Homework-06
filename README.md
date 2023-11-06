# CS569 Homework 
### Coding Exercise
In a new Angular application, create the following:  
  
  * Data service `data.service.ts`
  * List component `list.component.ts` (stateful/container)
  * Card component `card.component.ts` (stateless/representational)
  
Implementation details:  
1. Create a button on your root component to Show/Hide (Mount/Unmount) the `ListComponent` which is hidden by default. 
2. Your `DataService` has a method `getData()` that sends a GET request to the following URL `https://randomuser.me/api/?results=10`. Use the following tool to create a response type [JSON to TypeScript service](https://transform.tools/json-to-typescript)
  
3. When you mount `ListComponent`, call `getData()` method and display the list of cards (solve in two ways: subscribe and async pipe). Every user card should be displayed using `CardComponent`. 
4. The the `CardComponent` will display the user's picture, first and last name, date of birth, full address, and phone number. You may use [Flowbite](https://flowbite.com/docs/components/card/). ([Tailwind setup](https://flowbite.com/docs/getting-started/angular/))

5. Format the date of birth using `date` pipe.
6. Create a functional interceptor that modifies all the outgoing HTTP request headers with an iPhone 15 Pro Max, Safari's user agent `Mozilla/5.0 (iPhone; CPU iPhone OS 17_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.1 Mobile/15E148 Safari/604.1`
