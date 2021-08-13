# Socket-Relay-Chat-Protocol
[ documentation ]

It uses websockets.

The client connects to the server.

Server issues a join broadcast.

The following format is used to serialize messages:
```javascript
{
  timestamp: Numeric,
  text: String
}
```
Messages are sent to the server using a *push* message.
Server stats, online users are sent via the *stats* message.
