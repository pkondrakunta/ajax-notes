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


- `readyState`
    This property holds the status of the XMLHttpRequest.
[readyState_values](https://github.com/pkondrakunta/ajax-notes/blob/master/readme_assets/ready_state_values.png)

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