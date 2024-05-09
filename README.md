# JavaScript---Theory-Concepts
### Table of Contents

| No. | Questions                                                                                                                                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What are web sockets](#what-are-web-sockets)                                                                                           |
| 2   | [Output 1](#output-1)                                                   |
| 2   | [ Output 2](#output-2 )                                                   |

1. ### What are web sockets?
Websockets are a communication protocol that enables real-time, bidirectional communication between clients and servers over a single, long-lived connection. Unlike traditional HTTP requests, which follow a request-response pattern and require a new connection for each request, websockets maintain a persistent connection between the client and server, allowing both parties to send messages to each other asynchronously.
Websockets are commonly used in applications where real-time updates are required, such as chat applications, online gaming, collaborative editing tools, and financial trading platforms. They provide lower latency and overhead compared to traditional HTTP-based approaches for real-time communication.
One of the key advantages of websockets is their ability to push data from the server to the client without the need for the client to continually poll the server for updates. This makes them more efficient for applications that require frequent data updates or notifications.
Websockets are supported by most modern web browsers and are commonly used in conjunction with technologies such as JavaScript for client-side implementation and frameworks like Socket.IO for server-side implementation.

**[⬆ Back to Top](#table-of-contents)**
---
2. ### Output 1
 ```js
   getProjects().then(() => console.log('hi'));
      console.log('hello');
   ```
   The console.log('hello') statement will be executed first, followed by the .then() callback function (console.log('hi')).
This is because getProjects() is an asynchronous function that returns a Promise. When you call getProjects().then(), it schedules the execution of the callback function to be executed asynchronously after the promise returned by getProjects() resolves. Meanwhile, the console.log('hello') statement is synchronous and will be executed immediately.

**[⬆ Back to Top](#table-of-contents)**
---
3. ### Output 2
```js
await getProjects();
console.log('hello');
```
In JavaScript, when you use the await keyword, it pauses the execution of the code until the promise returned by the asynchronous function getProjects() resolves. This means that the code inside getProjects() will be executed first, and only after it completes will the console.log('hello') statement be executed. The output will be the result of getProjects() (assuming it returns something), followed by 'hello'

**[⬆ Back to Top](#table-of-contents)**
---

