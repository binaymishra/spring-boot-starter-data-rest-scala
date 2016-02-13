# spring-boot-starter-data-rest-scala
A small study project on how to use spring-boot-starter-data-rest

# TL;DR
With [spring-boot-starter-data-rest](http://docs.spring.io/spring-data/rest/docs/2.4.2.RELEASE/reference/html/) 
you can create hypermedia driven REST services with virtually no effort. 

Service | Status | Description
------- | ------ | -----------
License | [![License](http://img.shields.io/:license-Apache%202-red.svg)](http://www.apache.org/licenses/LICENSE-2.0.txt) | Apache 2.0

# Calling the web service
Service | Verb | [httpie](https://github.com/jkbrzt/httpie) | Description
--------|------|--------|-------------
/books    | GET  | http -v get localhost:8080/api/books | Get a list of books
/books    | POST | http -v post localhost:8080/api/books reader=foo isbn=bar id=0 | Create a book
/books/{id} | GET | http -v get localhost:8080/api/books/1 | Get a book by id
/books/{id}| DELETE | http -v delete localhost:8080/books/1 | Delete a book by id
/books | DELETE | http -v delete localhost:8080/api/books | Delete all books

# Resources
- [Spring Data REST](http://docs.spring.io/spring-data/rest/docs/2.4.2.RELEASE/reference/html/)
- [Common application properties](https://docs.spring.io/spring-boot/docs/current/reference/html/common-application-properties.html)

Have fun!