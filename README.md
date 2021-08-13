# Socket-Relay-Chat-Protocol
[ documentation ]

It uses websockets.

The client connects to the server.

Server issues a join broadcast.

The following format is used to serialize messages:

*push* message
```javascript
{
  timestamp: Numeric,
  text: String
}
```

*stats* message
```javascript
{
  connections: Numerical  // How many clients are online
}
```
