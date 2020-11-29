:black_heart: Google book search API (rest API)
prerequisite: VS code

No need a API key for searching books on google

### Process
* Open VS code and install `REST Client`(short cut for mac: shift + command + X)
<div>
<img width="1022" alt="rest_client" src="https://user-images.githubusercontent.com/40614421/100554507-599e6200-3295-11eb-8fd7-d1c63cf48642.png"> 
</div>

* Send an HTTP `GET` request to the following URI:
```
GET https://www.googleapis.com/books/v1/volumes?q={options}
```
* Specify your options after `https://www.googleapis.com/books/v1/volumes?q={options}`
<div>
<img width="1531" alt="google book APIs" src="https://user-images.githubusercontent.com/40614421/100554538-9407ff00-3295-11eb-9ec0-8755a16265d4.png">
</div>

```
GET https://www.googleapis.com/books/v1/volumes?q=La Reine Margot

###
GET https://www.googleapis.com/books/v1/volumes?q=L'etranger+inauthor:Albert Camus&download=epub

###

GET https://www.googleapis.com/books/v1/volumes?q=Alexandre Dumas&filter=free-ebooks
```
(short cut to send request for mac : option + command + R)
* 1st request : search a book titled `La Reine Margot`
* 2nd request : search a book titled `L'etranger` by author `Albert Camus` and ebook format `epub` only
* 3rd request : search `free-ebooks` by `Alexandre Dumas`


Check [Google Books APIs](https://developers.google.com/books/docs/v1/using#APIKey) to specify options.

If you feel like, clone the code, change options and search books.
```
git clone https://github.com/soyounson/APIs.git
```

Korean ref: [REST API개념, 구성요소, URL설계규칙, REST Client, API사용 실습](https://www.youtube.com/watch?v=X4DezEXbc5o)

Enjoy :)
