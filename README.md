:black_heart: Google book serch API (rest API)
prerequisite : VS code

Do not need a API key for searching books on google

### Process
* Open VS code and install `REST Client`(short cut for mac: shift + command + X).
* Send an HTTP `GET` request to the following URI:
```
GET https://www.googleapis.com/books/v1/volumes?q={options}
```
* Specify your options after `https://www.googleapis.com/books/v1/volumes?q={options}`

```
GET https://www.googleapis.com/books/v1/volumes?q=La Reine Margot

###
GET https://www.googleapis.com/books/v1/volumes?q=L'etranger+inauthor:Albert Camus&download=epub

###

GET https://www.googleapis.com/books/v1/volumes?q=Alexandre Dumas&filter=free-ebooks
```
* 1st request : search a book titled `La Reine Margot`
* 2nd request : search a book titled `L'etranger` by author `Albert Camus` and ebook format `epub` only
* 3rd request : search `free-ebooks` by `Alexandre Dumas`

Check [Google Books APIs](https://developers.google.com/books/docs/v1/using#APIKey) to specify options.

If you feel like, clone the code, change options and search books.
```
git clone https://github.com/soyounson/APIs.git
```

[ref in Korean](https://www.youtube.com/watch?v=X4DezEXbc5o)

Enjoy :)
