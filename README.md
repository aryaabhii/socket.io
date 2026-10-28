# Socket examples

This repository contains two small, independent Node.js examples. Each has its
own `package.json` and dependencies, so run commands from the example's folder.

## Requirements

- Node.js
- npm

## Express page (`socket.io/`)

This example serves a static page from `socket.io/public` using Express.

```powershell
cd socket.io
npm install
npm start
```

Open [http://localhost:9000](http://localhost:9000) in a browser. The current
page is a simple Chat App welcome screen; it does not yet implement Socket.IO
messaging.

## WebSocket echo server (`websocket/`)

This example uses Express and the `ws` package to run a WebSocket echo server.
Each message sent by a connected client is returned with an `Echo: ` prefix.

```powershell
cd websocket
npm install
npm start
```

The server listens on port `8080`. Connect a WebSocket client to
`ws://localhost:8080`, send a message such as `Hello`, and the server responds
with `Echo: Hello`. You can test it with
[Hoppscotch WebSocket](https://hoppscotch.io/realtime/websocket).

Press **Ctrl+C** in the server terminal to stop either example.
