# JavaScript---Theory-Concepts
### Table of Contents

| No. | Questions                                                                                                                                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What are web sockets](#what-are-web-sockets)                                                                                                                 |
| 2   | [What is a service worker](#what-is-a-service-worker )                                                                                                        |
| 3   | [ How do you manipulate DOM using a service worker ](#how-do-you-manipulate-dom-using-a-service-worker )                                                      |
| 4   | [ What is IndexedDB ](#what-is-indexeddb )                                                                                                                    |
| 5   | [ What is web storage ](#what-is-web-storage )                                                                                                                |
| 6   | [ What is a post message ](#what-is-a-post-message )                                                                                                          |
| 7   | [What are the options in a cookie ?](#what-are-the-options-in-a-cookie)                                                                                       |
| 8   | [ What are the methods available on session storage? ](#what-are-the-methods-available-on-session-storage )                                                   |
| 9   | [ What are server-sent events ](#what-are-server-sent-events )                                                                                                |
| 10  | [ What is the purpose of the delete operator in JavaScript? ](#what-is-the-purpose-of-the-delete-operator-in-javascript )                                     |
| 11  | [ How do you access history in javascript? ](#how-do-you-access-history-in-javascript )                                                                       |
| 12  | [ What is the difference between native, host and user objects? ](#what-is-the-difference-between-native-host-and-user-objects )                              |
| 13  | [ What is same-origin policy? ](#what-is-same-origin-policy )                                                                                                 |
| 14  | [ What is the purpose JSON stringify? ](#what-is-the-purpose-json-stringify )                                                                                 |
| 15  | [ How do you parse JSON string? ](#how-do-you-parse-json-string )                                                                                             |
| 16  | [ How do you test for length of object? ](#how-do-you-test-for-length-of-object )                                                                             |
| 17  | [ How do you check if a string starts with another string? ](#how-do-you-check-if-a-string-starts-with-another-string )                                       |
| 18  | [ What is tree shaking? ](#what-is-tree-shaking )                                                                                                             |
| 19  | [ What is the need of tree shaking? ](#what-is-the-need-of-tree-shaking )                                                                                     |
| 20  | [ What is the purpose of double exclamation? ](#what-is-the-purpose-of-double-exclamation )                                                                   |
| 21  | [ How do you determine two values same or not using object? ](#how-do-you-determine-two-values-same-or-not-using-object )                                     |
| 22  | [ How do you copy properties from one object to other? ](#how-do-you-copy-properties-from-one-object-to-other )                                               |
| 23  | [ What is the purpose of seal method? ](#what-is-the-purpose-of-seal-method )                                                                                 |
| 24  | [ What are the differences between freeze and seal methods? ](#what-are-the-differences-between-freeze-and-seal-methods )                                     |
| 25  | [ What are the differences between WeakSet and Set? ](#what-are-the-differences-between-weakset-and-set )                                                     |
| 26  | [ What is the output of below spread operator array? ](#what-is-the-output-of-below-spread-operator-array )                                                   |
| 27  | [ How do you combine two or more arrays? ](#how-do-you-combine-two-or-more-arrays )                                                                           |
| 28  | [ What is the output of below console statement with unary operator? ](#what-is-the-output-of-below-console-statement-with-unary-operator )                   |
| 29  | [ What happens if we add two arrays? ](#what-happens-if-we-add-two-arrays )                                                                                   |
| 30  | [ How do you empty an array? ](#how-do-you-empty-an-array )                                                                                                   |
| 31  | [  ](# )                                                          |
| 32  | [  ](# )                                                          |

1. ### What are web sockets?
Websockets are a communication protocol that enables real-time, bidirectional communication between clients and servers over a single, long-lived connection. Unlike traditional HTTP requests, which follow a request-response pattern and require a new connection for each request, websockets maintain a persistent connection between the client and server, allowing both parties to send messages to each other asynchronously.
Websockets are commonly used in applications where real-time updates are required, such as chat applications, online gaming, collaborative editing tools, and financial trading platforms. They provide lower latency and overhead compared to traditional HTTP-based approaches for real-time communication.
One of the key advantages of websockets is their ability to push data from the server to the client without the need for the client to continually poll the server for updates. This makes them more efficient for applications that require frequent data updates or notifications.
Websockets are supported by most modern web browsers and are commonly used in conjunction with technologies such as JavaScript for client-side implementation and frameworks like Socket.IO for server-side implementation.

**[⬆ Back to Top](#table-of-contents)**
---


2. ### What is a service worker
   A Service worker is basically a script (JavaScript file) that runs in the background, separate from a web page and provides features that don't need a web page or user interaction. 
   Some of the major features of service workers are Rich offline experiences(offline first web application development), periodic background syncs, push notifications, intercept and 
   handle network requests and programmatically managing a cache of responses.
   
**[⬆ Back to Top](#table-of-contents)**
---
3. ### How do you manipulate DOM using a service worker
   Service worker can't access the DOM directly. But it can communicate with the pages it controls by responding to messages sent via the postMessage interface, and those pages can 
   manipulate the DOM.
   
**[⬆ Back to Top](#table-of-contents)**
---

4. ### What is IndexedDB
   IndexedDB is a low-level API for client-side storage of larger amounts of structured data, including files/blobs. This API uses indexes to enable high-performance searches of this 
   data.
   
**[⬆ Back to Top](#table-of-contents)**
---
5. ### What is web storage
   Web storage is an API that provides a mechanism by which browsers can store key/value pairs locally within the user's browser, in a much more intuitive fashion than using cookies. 
   The web storage provides two mechanisms for storing data on the client.
   Local storage: It stores data for current origin with no expiration date.
   Session storage: It stores data for one session and the data is lost when the browser tab is closed.
   
**[⬆ Back to Top](#table-of-contents)**
---

6. ### What is a post message
    Post message is a method that enables cross-origin communication between Window objects.(i.e, between a page and a pop-up that it spawned, or between a page and an iframe embedded 
    within it). Generally, scripts on different pages are allowed to access each other if and only if the pages follow same-origin policy(i.e, pages share the same protocol, port 
    number, and host).
   
**[⬆ Back to Top](#table-of-contents)**
---
7. ### What are the options in a cookie?
There are few below options available for a cookie,
By default, the cookie is deleted when the browser is closed but you can change this behavior by setting expiry date (in UTC time).
document.cookie = "username=John; expires=Sat, 8 Jun 2019 12:00:00 UTC";

By default, the cookie belongs to a current page. But you can tell the browser what path the cookie belongs to using a path parameter.
document.cookie = "username=John; path=/services";

**[⬆ Back to Top](#table-of-contents)**
---
8. ### What are the methods available on session storage?
   The session storage provided methods for reading, writing and clearing the session data
   
_Save data to sessionStorage_
sessionStorage.setItem("key", "value");

_Get saved data from sessionStorage_
let data = sessionStorage.getItem("key");

_Remove saved data from sessionStorage_
sessionStorage.removeItem("key");

_Remove all saved data from sessionStorage_
sessionStorage.clear();

**[⬆ Back to Top](#table-of-contents)**
---
9. ### what-are-server-sent-events ?
    Server-sent events (SSE) is a server push technology enabling a browser to receive automatic updates from a server via HTTP connection without resorting to polling. These are a one way communications channel - events flow from server to client only. This has been used in Facebook/Twitter updates, stock price updates, news feeds etc.

**[⬆ Back to Top](#table-of-contents)**
---
10. ### What is the purpose of the delete operator in JavaScript?
The delete operator is used to delete the property as well as its value.
var user = { firstName: "John", lastName:"Doe", age: 20 };
delete user.age;

console.log(user); // _{firstName: "John", lastName:"Doe"}_

**[⬆ Back to Top](#table-of-contents)**
---
11. ### How do you access history in javascript?
The window.history object contains the browser's history. You can load previous and next URLs in the history using back() and next() methods.
function goBack() {
  window.history.back();
}
function goForward() {
  window.history.forward();
}

Note: You can also access history without window prefix.

**[⬆ Back to Top](#table-of-contents)**
---
12. ### What is the difference between native, host and user objects?
    Native objects are objects that are part of the JavaScript language defined by the ECMAScript specification. For example, String, Math, RegExp, Object, Function etc core objects defined in the ECMAScript spec. 

Host objects are objects provided by the browser or runtime environment (Node). For example, window, XmlHttpRequest, DOM nodes etc are considered as host objects.

 User objects are objects defined in the javascript code. For example, User objects created for profile information.

**[⬆ Back to Top](#table-of-contents)**
---
13. ### What is same-origin policy?
    The same-origin policy is a policy that prevents JavaScript from making requests across domain boundaries. An origin is defined as a combination of URI scheme, hostname, and port number. If you enable this policy then it prevents a malicious script on one page from obtaining access to sensitive data on another web page using Document Object Model(DOM).

**[⬆ Back to Top](#table-of-contents)**
---
14. ### What is the purpose JSON stringify?
    When sending data to a web server, the data has to be in a string format. You can achieve this by converting JSON object into a string using stringify() method.
var userJSON = { name: "John", age: 31 };
var userString = JSON.stringify(userJSON);
console.log(userString); // _"{"name":"John","age":31}"_

**[⬆ Back to Top](#table-of-contents)**
---
15. ### How do you parse JSON string?
When receiving the data from a web server, the data is always in a string format. But you can convert this string value to a javascript object using parse() method.
var userString = '{"name":"John","age":31}';
var userJSON = JSON.parse(userString);
console.log(userJSON); // {name: "John", age: 31}

**[⬆ Back to Top](#table-of-contents)**
---
16. ### How do you test for length of object?
console.log(Object.entries(alok).length)

17. ### How do you check if a string starts with another string?
    You can use ECMAScript 6's String.prototype.startsWith() method to check if a string starts with another string or not. But it is not yet supported in all browsers. Let's see an example to see this usage,
"Good morning".startsWith("Good"); // true
"Good morning".startsWith("morning"); // false

**[⬆ Back to Top](#table-of-contents)**
---
18. ### What is tree shaking?
Tree shaking is a form of dead code elimination. It means that unused modules will not be included in the bundle during the build process and for that it relies on the static structure of ES2015 module syntax,( i.e. import and export). Initially this has been popularized by the ES2015 module bundler rollup.

**[⬆ Back to Top](#table-of-contents)**
---
19. ### What is the need of tree shaking?
Tree Shaking can significantly reduce the code size in any application. i.e, The less code we send over the wire the more performant the application will be. For example, if we just want to create a “Hello World” Application using SPA frameworks then it will take around a few MBs, but by tree shaking it can bring down the size to just a few hundred KBs. Tree shaking is implemented in Rollup and Webpack bundlers.

20. ### What is the purpose of double exclamation?
The double exclamation or negation(!!) ensures the resulting type is a boolean. If it was falsey (e.g. 0, null, undefined, etc.), it will be false, otherwise, it will be true. For example, you can test IE version using this expression as below,
let isIE8 = false;
isIE8 = !!navigator.userAgent.match(/MSIE 8.0/);
console.log(isIE8); // returns true or false

**[⬆ Back to Top](#table-of-contents)**
---
21. ### How do you determine two values same or not using object?
The Object.is() method determines whether two values are the same value. For example, the usage with different types of values would be,
Object.is("hello", "hello"); // true
Object.is(window, window); // true
Object.is([], []); // false

**[⬆ Back to Top](#table-of-contents)**
---
22. ### How do you copy properties from one object to other?
You can use the Object.assign() method which is used to copy the values and properties from one or more source objects to a target object. It returns the target object which has properties and values copied from the source objects. The syntax would be as below,
Object.assign(target, ...sources);

_Let's take example with one source and one target object_ ,
const target = { a: 1, b: 2 };
const source = { b: 3, c: 4 };

const returnedTarget = Object.assign(target, source);

console.log(target); // { a: 1, b: 3, c: 4 }

console.log(returnedTarget); // { a: 1, b: 3, c: 4 }

23. ### What is the purpose of seal method?
The Object.seal() method is used to seal an object, by preventing new properties from being added to it and marking all existing properties as non-configurable. But values of present properties can still be changed as long as they are writable. Let's see the below example to understand more about seal() method
const object = {
  property: "Welcome JS world",
};
Object.seal(object);
object.property = "Welcome to object world";
console.log(Object.isSealed(object)); // true
delete object.property; // You cannot delete when sealed
console.log(object.property); //Welcome to object world

**[⬆ Back to Top](#table-of-contents)**
---
24. ### What are the differences between freeze and seal methods?
If an object is frozen using the Object.freeze() method then its properties become immutable and no changes can be made in them whereas if an object is sealed using the Object.seal() method then the changes can be made in the existing properties of the object.

**[⬆ Back to Top](#table-of-contents)**
---
25. ### What are the differences between WeakSet and Set?
The main difference is that references to objects in Set are strong while references to objects in WeakSet are weak. i.e, An object in WeakSet can be garbage collected if there is no other reference to it. Other differences are,
* Sets can store any value Whereas WeakSets can store only collections of objects
* WeakSet does not have size property unlike Set
* WeakSet does not have methods such as clear, keys, values, entries, forEach.
* WeakSet is not iterable.

**[⬆ Back to Top](#table-of-contents)**
---
26. ### What is the output of below spread operator array?
[..."John Resig"];

The output of the array is ['J', 'o', 'h', 'n', '', 'R', 'e', 's', 'i', 'g'] Explanation: The string is an iterable type and the spread operator within an array maps every character of an iterable to one element. Hence, each character of a string becomes an element within an Array.

**[⬆ Back to Top](#table-of-contents)**
---
27. ### How do you combine two or more arrays?
The concat() method is used to join two or more arrays by returning a new array containing all the elements. The syntax would be as below,
array1.concat(array2, array3, ..., arrayX)

Let's take an example of array's concatenation with veggies and fruits arrays,
var veggies = ["Tomato", "Carrot", "Cabbage"];
var fruits = ["Apple", "Orange", "Pears"];
var veggiesAndFruits = veggies.concat(fruits);
console.log(veggiesAndFruits); // Tomato, Carrot, Cabbage, Apple, Orange, Pears

**[⬆ Back to Top](#table-of-contents)**
---
28. ### What is the output of below console statement with unary operator?
Let's take console statement with unary operator as given below,
console.log(+"Hello");

The output of the above console log statement returns NaN. Because the element is prefixed by the unary operator and the JavaScript interpreter will try to convert that element into a number type. Since the conversion fails, the value of the statement results in NaN value.

**[⬆ Back to Top](#table-of-contents)**
---
29. ### What happens if we add two arrays?
If you add two arrays together, it will convert them both to strings and concatenate them. For example, the result of adding arrays would be as below,
console.log(["a"] + ["b"]); // "ab"
console.log([] + []); // ""
console.log(![] + []); // "false", because ![] returns false.

**[⬆ Back to Top](#table-of-contents)**
---
30. ### How do you empty an array?
You can empty an array quickly by setting the array length to zero.
let cities = ["Singapore", "Delhi", "London"];
cities.length = 0; // cities becomes []





