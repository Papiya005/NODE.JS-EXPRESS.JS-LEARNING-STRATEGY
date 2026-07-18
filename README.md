# 🚀 Node.js & Express.js Learning Journey

<p align="center">
  <img src="https://nodejs.org/static/images/logo.svg" alt="Node.js Logo" width="200">
</p>

## 📖 Overview

This repository contains my notes, practice programs, and mini-projects created while learning **Node.js** and **Express.js**. The repository documents my backend development journey and serves as a reference for concepts, code examples, and projects.

---

## 🛠️ Technologies Used

<p align="center">
  <img src="https://skillicons.dev/icons?i=nodejs,express,js,npm,git,github,vscode" />
</p>

---

# 🚀 What I Learned in Node.js & Express.js

## 📌 Node.js Fundamentals

* 🟢 Learned what Node.js is and how it allows JavaScript to run outside the browser.
* 🟢 Understood the role of the V8 Engine.
* 🟢 Learned about built-in modules such as:

  * 📂 `fs` (File System)
  * 🛣️ `path`
  * 💻 `os`
* 🟢 Learned how to import and export modules using:

  * `require()`
  * `module.exports`
* 🟢 Learned package management using npm.
* 🟢 Worked with `package.json` and project initialization.

---

## 🌐 Express.js Fundamentals

* 🟢 Created web servers using Express.js.
* 🟢 Understood how Express simplifies backend development.
* 🟢 Learned how client requests are processed and responses are returned.

---

## 🛣️ Routing

* 🟢 Created routes using:

  * `app.get()`
  * `app.post()`
  * `app.put()`
  * `app.delete()`

* 🟢 Understood that routes execute only when:

  * The URL path matches.
  * The HTTP method matches.

Example:

```js
app.get("/", (req, res) => {
    res.send("Home Page");
});
```

---

## ⚙️ Middleware

* 🟢 Learned the concept of middleware.
* 🟢 Understood that middleware executes between the request and response cycle.
* 🟢 Learned the purpose of:

  * 📥 `req` → Request Object
  * 📤 `res` → Response Object
  * ➡️ `next()` → Pass control to the next middleware or route

Example:

```js
app.use((req, res, next) => {
    console.log("Request Received");
    next();
});
```

---

## 🔄 Understanding `app.use()`

* 🟢 Learned how to register middleware using `app.use()`.
* 🟢 Understood that it works with all HTTP methods.
* 🟢 Learned route-prefix middleware.

Example:

```js
app.use("/admin", (req, res, next) => {
    next();
});
```

Matches:

```text
/admin
/admin/profile
/admin/settings
```

---

## 📡 Understanding `app.get()`

* 🟢 Learned that `app.get()` handles only GET requests.
* 🟢 Understood that it executes when:

  * The request method is GET.
  * The route path matches.

Example:

```js
app.get("/user", (req, res) => {
    res.send("User Data");
});
```

---

## 🔀 Express Request Flow

```text
📥 Client Request
        ↓
⚙️ Middleware
        ↓
⚙️ Middleware
        ↓
🛣️ Route Handler
        ↓
📤 Response
```

---

## 📋 Request Data Handling

* 🟢 Learned about:

  * `req.params`
  * `req.query`
  * `req.body`

* 🟢 Understood how to access data sent by the client.

---

## 📤 Response Handling

* 🟢 Learned how to send responses using:

  * `res.send()`
  * `res.json()`
  * `res.status()`

* 🟢 Understood that `res.send()` ends the request-response cycle.

---

## 🎯 Key Concepts Mastered

* ✅ Node.js Basics
* ✅ Express.js Fundamentals
* ✅ Server Creation
* ✅ Routing
* ✅ Middleware
* ✅ Route Matching
* ✅ HTTP Methods
* ✅ Request & Response Objects
* ✅ `next()` Function
* ✅ Request Lifecycle
* ✅ npm & Package Management
* ✅ Module System (`require` & `module.exports`)

---

## 🚧 Next Topics to Learn

* 📄 EJS (Template Engine)
* 🗄️ MongoDB
* 🔗 Mongoose
* 🔐 Authentication & Authorization
* 🍪 Cookies & Sessions
* 🌍 REST APIs
* ☁️ Deployment


---

## 👩‍💻 Author

**Papiya Dutta**

* GitHub: https://github.com/Papiya005
* LinkedIn: https://linkedin.com/in/papiya-dutta-43786131b
