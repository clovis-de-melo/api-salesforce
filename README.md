# API & Salesforce

### What is an API?

APIs are mechanisms that enable two software components to communicate with each other using a set of definitions and protocols. For example, the weather bureau’s software system contains daily weather data. The weather app on your phone “talks” to this system via APIs and shows you daily weather updates on your phone.


### What does API stand for? 

API stands for *Application Programming Language*. In the context of APIs, the word *Application* refers to any software with a distinct function. *Interface* can be thought of as a contract of service between two applications. This contract defines how the two communicate with each other using requests and responses. Their API documentation contains information on how developers are to structure those requests and responses.

### Types of API

#### REST ####





### HTTP Request Methods or Verbs

HTTP (*Hypertext Transfer Protocol*) defines a set of request methods to indicate the purpose of the request and what is expected if the request is successful. Although they can also be nouns, these request methods are sometimes referred to as HTTP verbs. Each request method has its own semantics, but some characteristics are shared across multiple methods, specifically request methods can be safe, idempotent, or cacheable.

#### GET ####

The *GET* method is used to request data from a specified resource.

Follows below a simple HTTP Get request example: 

`GET /home/user/example.txt HTTP/1.1`

Some notes on GET requests: 

* GET requests can be cached
* GET requests remain in the browser history
* GET requests can be bookmarked
* GET requests should never be used when dealing with sensitive data
* GET requests have length restrictions
* GET requests are only used to request data (not modify)

#### POST ####

The *POST* method is used to send data to a server to create/update a resource.

The data sent to the server with POST is stored in the request body of the HTTP request.

Follows below some examples of POST method:

```
POST /test/demo_form.php HTTP/1.1
Host: w3schools.com

name1=value1&name2=value2
```

````
POST /home/user/datafile HTTP/1.1
From: user@linode33
User-Agent: Mytools/0.8.0
Content-Type: application/json
Content-Length: 32

{
    [Json-formatted data pairs]
}

````

#### Head ####

The *HEAD* method submits an entity to the specified resource, often causing a change in state or side effects on the server.





#### Put ####

The *PUT* method replaces all current representations of the target resource with the request [content](https://developer.mozilla.org/en-US/docs/Glossary/HTTP_Content) (or information).

#### Delete ####

#### Connect ####

#### Options ####

#### Trace ####

#### Patch ####


## Salesforce APIs

![Salesforce APIs](images/Salesforce%20APIs%20-%20Integrate%20applications%20with%20Salesforce.png)

### What is Apex? 

Apex is a strongly typed, *object-oriented programming language* that allows developers to execute flow and transaction control statements on Salesforce servers in conjunction with calls to the API. Using syntax that looks like Java and acts like database stored procedures, Apex enables developers to add business logic to most system events, including button clicks, related record updates, and Visualforce pages. Apex code can be initiated by Web service requests and from triggers on objects.

### Apex class

An Apex class is a template or blueprint from which Apex objects are created. Classes consist of other classes, user-defined methods, variables, exception types, and static initialization code.

### What does CLI stands for? 




### Salesforce ORG aka Playground


## Keywords 

`HTTP`

HTTP stands for *Hypertext Transfer Protocol*. It's a set of rules that allow web browsers and servers to communicate with each other. HTTP is the foundation of the World Wide Web.

How HTTP works: 

* A web browser sends a HTTP request to a server.
* The server sends a HTTP response back to the browser.
* The browser is called the "client" and the server-browser relationship is called a "client-server" relationship.

`CRUD`

*C*reate, *R*ead, *U*pdate, *D*elete are the four basic functions that models should be able to do, at most.


`cURL`

The name "curl" stands for *Client for URL*. Is a command-line tool and library for transferring data with URLs. It was originally developed by Daniel Stenberg and has become one of the most versatile and powerful utilities for data transfer over the Internet

`SDK`

 A *software development kit* (SDK) is a set of platform-specific building tools for developers. You require components like debuggers, compilers, and libraries to create code that runs on a specific platform, operating system, or programming language. SDKs put everything you need to develop and run software in one place. Additionally, they contain resources like documentation, tutorials, and guides as well as APIs and frameworks for faster application development.

`Webhoock`



`Auoth 2.0`


`PubSub architecture`


`Endpoint`




## References

`Salesforce`

[Salesforce Trailhead | API basics](https://trailhead.salesforce.com/content/learn/modules/pw-api-basics)

[Salesforce Developers | What is Apex?](https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_intro_what_is_apex.htm)

[Salesforce Developers | Apex meta classes](https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_classes.htm)

[Salesforce Developers | CLI installation](https://developer.salesforce.com/tools/salesforcecli)

`AWS`

[AWS | What is an API? ](https://aws.amazon.com/what-is/api/)

[AWS | What is an SDK?](https://aws.amazon.com/what-is/sdk/)

`Codecademy`

[Codecademy | What is Crud?](https://www.codecademy.com/article/what-is-crud)


`MDN Web Docs`

[MDN Web Docs | HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP)

[MDN Web Docs | HTTP Request Methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)