[client] - send a request -> [server] - send a response -> [client]

[client] - send a request -> [DNS Server] -> [CDN] -> [server] - send a response -> [client]

| Not RESTful             | RESTful                                                     |
| ----------------------- | ----------------------------------------------------------- |
| `/createHubs`           | POST `/hubs`                                                |
| `/listHubMessages/:id`  | GET `/hubs/:id/messages`                                    |
| `/countHubMessages/:id` | GET `/hubs/:id/messages` add a `count` prop to the response |

Separation of Concerns

https://www.google.com/search <- url
? <- marks the beginning of the `query string`
newwindow=1 <- key value pair with parameters
& <- key/value pair separator
source <- key
=
hp <- value
&
ei=9CiRXK_fG-PojwTlu67QDg

```js
const query = {
  newwindow: 1,
  source: hp,
};
```



http://localhost:4000/api/hubs?limit=5&page=2&sortby=name&sortdir=decs