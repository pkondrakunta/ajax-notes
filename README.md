# Learning AJAX


DOM Manipulation (Document Object Manipulation):

Steps in Javascript:
- Traverse 
- Manipulate

There are two steps. Ensure that the required elements are being selected. You cannot manipulate until you select.


### How do you make your application RIA (Rich Internet Application)?
By using:
- HTML5
- CSS3
- JavaScript
- AJAX

## Why do we need JavaScript in AJAX request?

Steps to using JS in your application:
1. Event Handler
2. To create XML Http request object
3. Send the request to the server
4. DOM traversal 
5. DOM manipulation

## Important properties of XMLHttpRequest

There are three properties of xmlHttprequest that we need to know:
- `onreadystatechange`
    This is a property that points to a function every time the state changes

```js
var xmlhttprequest = new XMLHttpRequest();

xmlhttprequest.onreadystatechange = function(){
    //Code here
}
```
- `readyState`

[./readme_assets/ready_state_values.png](./readme_assets/ready_state_values.png)
