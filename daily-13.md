# Local Storage

## What we really want?
- A lot of storage space
- On the client
- That persists beyond a page refresh
- And isn't transmitted to the server

## Intro HTML5 storage
- "HTML5 Storage" is web Storage
- What is it? A way for web pages to store named key/value pairs locally, within the client web browser. 
- This data stays even after you stay

## Using HTML5 Storage
- Based on named key/value pairs
- Store with the name key then you can retrieve it later with the same key name
- `setItem()`
- `getItem()`
- In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash Cookies” The feature is properly known as Local Shared Objects.
- Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks.
- The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database.