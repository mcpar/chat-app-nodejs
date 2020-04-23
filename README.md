# Chat App on Node.js

A simple web chat based on socket.io and Node.js

## Tech Stack

- [Node.js](https://nodejs.org/en/download/) - JavaScript runtime Server
- [Express.js](https://expressjs.com/) - Web framework
- [HandleBars](https://handlebarsjs.com/) - View Engine
- [Socket.io](https://socket.io/) - Real Time Engine based on WebSockets
- [Bulma](https://bulma.io/) - CSS framework.

### Setup

- Install [Node](https://nodejs.org/en/download/).
- Clone the [repo](https://github.com/jocnjr/chat-app-nodejs) or download the [zip file](https://github.com/jocnjr/chat-app-nodejs/archive/master.zip).

```
$ npm install
$ npm start
$ open http://localhost:3000/
```

Open the browser [http://localhost:3000](http://localhost:3000).

### 1 - The Basics

Understand the basic data exchange between server and client using socket.

We'll undestand how Node.js deals with events and exchange data.

### 2 - The Timer

We'll send random data and percieve the "real time" feeling.

### 3 - The Chat

Finally. Here's the chat:

- sending data from html from input
- broadcast data back to all clients

Replace this code on your index.hbs file at: views/index.hbs

```
<section class="section">
  <div class="container-fluid">
    <h1 class="title">
      {{title}}
    </h1>
    <p class="subtitle">
      welcome to {{title}}!
    </p>
    <div class="content" id="message"></div>
    <hr>
    <div class="field">
      <div class="control">
        <input class="input is-primary is-medium" type="text" name="message" placeholder="type your message">
      </div>
    </div>
    <button class="button is-primary">Send Message</button>
    <br>
    <div id="watch_mouse"></div>
  </div>
</section>

```
