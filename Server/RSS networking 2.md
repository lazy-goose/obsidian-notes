MPA - Multi Page Application
AJAX - Async Javascript and XML - approach of web development without page reloading

Keep-Alive up to 6 requests

HTTP-1.1 vs HTTP-2
- 6 requests at the same time, others are waiting
- has no encoding (many headers + cookie)
- one-directional (Pull-request, 1 request - 3 responses)
- textual protocol -> binary

--
may not rewrite frontend

--
REST???

REST - Representational state transfer: architectrul style for implementing API

1 - Client-server: server is different from client, API
2 - Statelessness: independent requests, they do not know each other], only client contains all necessart information
3 - Cacheability
4 - Layered system: API hides complexity
5 - Code on demand (Optional): server can extend client by transfer executable code
6 - Uniform interface
  6.1 - Resource identification in request (indetificated by url)
  6.2 - Resource manipulation through implementation (should be enough information to change entry)
  6.3 - Self-descriptive messages (Accept, Content-Type)
  6.4 - Hypermedia as the engine of application state (HATEOAS)

URI -> (URL + URN, URL, URN)
|_ URL -> link, where
|_ URN -> name, what (do not used in web)

api/v1-wrong/NOT_GET_POSTS
api/v2-good/posts?limit=25&page=1 (use GET,POST,...)
api/v2-good/posts/:id