# webrtc-call-rooms

A lightweight, browser-only WebRTC calling-room demo built with HTML, Tailwind CSS, and JavaScript.

## Run

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080` in separate browser tabs. Rooms, passwords, participant presence, and WebRTC signaling are shared through browser storage and `BroadcastChannel` on the same origin.

## Important limitation

This implementation is intended for same-browser/same-origin testing. Native `localStorage` and `BroadcastChannel` do not connect separate devices or browsers. A real deployment needs a signaling server (WebSocket or WebRTC-compatible backend) for users on different computers.
