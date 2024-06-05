# JavaScript---Theory-Concepts
### Table of Contents

| No. | Questions                                                                                                                                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What are web sockets](#what-are-web-sockets)                                                                           |
| 2   | [What is a service worker](#what-is-a-service-worker )                                                                  |
| 3   | [ How do you manipulate DOM using a service worker ](#how-do-you-manipulate-dom-using-a-service-worker )                |
| 4   | [ What is IndexedDB ](#what-is-indexeddb )                                                                              |
| 5   | [ What is web storage ](#what-is-web-storage )                                                                          |
| 6   | [ What is a post message ](#what-is-a-post-message )                                                                    |
| 7   | [ What is a browser? ](#what-is-a-browser )                                                   |
| 8  | [  ](# )                                                   |
|    | [  ](# )                                                   |

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
7. ### <span style="color: blue;">What is a browser?</span>

**[⬆ Back to Top](#table-of-contents)**
---

