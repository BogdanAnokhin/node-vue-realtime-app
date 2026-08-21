# 💻 LearnNode

A learning project focused on **Node.js, Vue.js, WebSockets, web scraping and modern JavaScript tooling**.

The project was created to practice building web applications with a frontend/backend architecture and working with external web data.

## ✨ Features

* ⚡ Vue 3 frontend
* 🟢 Node.js backend
* 🚀 Express server
* 🔌 Real-time communication with WebSockets
* 🌐 Web scraping with Axios and Cheerio
* 📦 Webpack development and production builds
* 🎨 SCSS styling
* 🗺️ Leaflet integration
* 💬 Real-time chat functionality
* 💾 Local caching of scraped data

## 🛠️ Technologies

| Technology | Purpose                     |
| ---------- | --------------------------- |
| JavaScript | Main programming language   |
| Vue 3      | Frontend framework          |
| Node.js    | Backend/runtime             |
| Express    | HTTP server                 |
| WebSocket  | Real-time communication     |
| Axios      | HTTP requests               |
| Cheerio    | HTML parsing / web scraping |
| Webpack    | Bundling and development    |
| SCSS       | Styling                     |
| Bulma      | UI components               |
| Leaflet    | Interactive maps            |
| Nodemon    | Development server          |

## 📂 Project Structure

```text
Ta23blearnnode/
├── public/
│
├── src/
│   ├── comp/
│   ├── components/
│   ├── pages/
│   ├── App.vue
│   ├── Chat.vue
│   ├── index.html
│   ├── index.js
│   ├── server.js
│   └── style.scss
│
├── .vscode/
├── scrapeSMBC.js
├── scrapeWUMO.js
├── scrapeXKCD.js
├── server.js
├── webpack.config.js
├── package.json
└── readme.md
```

## 🔌 WebSocket Server

The project includes a WebSocket server built with the `ws` package.

The server runs on:

```text
ws://localhost:8080
```

It accepts JSON messages from connected clients and broadcasts received messages to other connected clients.

The server also keeps messages in memory and sends the existing messages to a newly connected client.

## 💬 Chat

The Vue frontend includes a real-time chat interface connected to the WebSocket server.

Example message flow:

```text
Vue Client
    │
    │ JSON message
    ▼
WebSocket Server
    │
    ├──► Client 1
    ├──► Client 2
    └──► Client 3
```

This part of the project was created to practice real-time client-server communication.

## 🌐 Web Scraping

The project contains several scraping scripts:

### XKCD

`scrapeXKCD.js` downloads XKCD comic pages, parses their HTML with Cheerio and extracts:

* Comic ID
* Image URL
* Title
* Description/text

The script also implements a local HTML cache to avoid downloading the same pages repeatedly.

### WUMO

`scrapeWUMO.js` demonstrates a similar scraping workflow with caching and HTML parsing.

### SMBC

`scrapeSMBC.js` retrieves the current comic from SMBC and extracts its image URL, title and alt text.

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/BogdanAnokhin/Ta23blearnnode.git
cd Ta23blearnnode
```

Install dependencies:

```bash
npm install
```

## 🚀 Development

### Start Webpack development server

```bash
npm run serve
```

### Build for production

```bash
npm run build
```

### Run WebSocket server

```bash
npm run express
```

## 🧪 Learning Goals

This project was created as a practical learning project to improve my understanding of:

* JavaScript modules
* Vue 3
* Node.js
* Express
* WebSockets
* HTTP requests
* Web scraping
* HTML parsing
* Webpack
* Client-server communication
* Asynchronous JavaScript
* File system operations
* Caching

## 📚 What I Learned

While working on this project, I practiced building applications where the frontend communicates with a backend in real time.

I also learned how to retrieve and process data from external websites, parse HTML using Cheerio and store cached results locally.

## 🔮 Future Improvements

* [ ] Add user authentication
* [ ] Store chat messages in a database
* [ ] Add persistent chat history
* [ ] Improve error handling
* [ ] Add environment variables for configuration
* [ ] Add automated tests
* [ ] Improve responsive design
* [ ] Deploy the application
* [ ] Add screenshots and demo GIFs

## 👨‍💻 Author

**Bogdan Anokhin**

Junior Software Developer
Tallinna Polütehnikum

[GitHub](https://github.com/BogdanAnokhin)
