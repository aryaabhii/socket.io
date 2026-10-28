# WebSocket Echo Server

A small WebSocket server built with Node.js, Express, and the `ws` package. It listens on port `8080` and sends each connected client an `Echo: ` response for every message it receives.

## Requirements

- Node.js 18 or later
- npm

## Run the server

From the project directory, install dependencies and start the server:

```powershell
npm install
npm start
```

The server listens on `http://localhost:8080`. Keep this terminal open while testing.

## Test with Hoppscotch

1. Open [Hoppscotch WebSocket](https://hoppscotch.io/realtime/websocket).
2. In the connection URL field, enter:

   ```text
   ws://localhost:8080
   ```

3. Click **Connect**.
4. Send a message, for example `Hello`.
5. The server replies with `Echo: Hello`.

The Hoppscotch page URL is an HTTPS web page; the WebSocket server address to connect to is `ws://localhost:8080`.

To stop the server, press **Ctrl+C** in the terminal running it.
