# Learning AJAX - Asynchronous JavaScript XML 

(you can also use JSON instead of XML but it is still called AJAX)

It is a technique that allows JavaScript to communicate with the server side. DOM manipulation with server response (there is DOM manipulation with JavaScript, don’t confuse that with the server side response).

It is used to refresh certain parts of the page instead of waiting for synchronous responses to a synchronous request. In order to use AJAX you need a special object, the XML HTTP request.

![AJAX Requests](https://github.com/pkondrakunta/ajax-notes/blob/master/readme_assets/ajax_requests.jpg)

> Using ID to traverse the tree is the worst (according to the professor). One of the best ways is to use neither ID nor tag name or class names. You can use selectors. 

> How do we use the following?\
    CSS
    - Traverse and style it\
    Javascript 
    - Traverse and manipulate it


DOM Manipulation (Document Object Manipulation). There are two steps for DOM manipulation in JS 
- Traverse 
- Manipulate

> Ensure that the required elements are being selected. You cannot manipulate until you select.


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


- `readyState`
    This property holds the status of the XMLHttpRequest.
![readyState_values](https://github.com/pkondrakunta/ajax-notes/blob/master/readme_assets/ready_state_values.png)

- `responseText`
    The data retrieved from the server will be stored in this property.

```js
xmlhttprequest.onreadystatechange = function(){
    if(xmlhttprequest.readyState == 4 && xmlhttprequest.status == 200){

        divElement.innerHTML = xmlhttprequest.responseText;
    }
}
```

## My ajaxservice.jsp

```jsp
<%
    String email = request.getParameter("email");
    out.println("Server Response at " + new java.util.Date());

%>
```

# jQuery

50% of jQuery is simply selecting the element `$(selector)`
Remaining 50% is built-in functions

`$(this)` represents the object that caused the instance

[jQuery API Reference](https://api.jquery.com/)

