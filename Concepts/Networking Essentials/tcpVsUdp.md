# TCP vs UDP

---

## TCP (Transmission Control Protocol)

**Connection-oriented**: Requires a handshake to establish a connection.
**Reliable**: Guarantees delivery through acknowledgments and retransmissions.
**Ordered**: Data packets are received in the exact order sent.
**Error-checking**: Ensures accuracy during transmission.
**Slower**, due to added overhead but ensures data integrity.

---

### Real-life Example: Online Exam

You’re taking a timed coding test online.

Every character and symbol you type must be received exactly.
If even one bracket is lost or out of order, your answer is incorrect.
Minor delay is acceptable — **accuracy is critical**.

**TCP is used** because it prioritizes reliability and order.

---


## UDP (User Datagram Protocol)

**Connectionless**: Sends data without establishing a connection.
**Unreliable**: No guarantee of delivery or order.
**Lightweight & Fast**: Minimal overhead, lower latency.
**No retransmission**, suitable for real-time communication.

---

### Real-life Example: Live Football Stream

You’re watching a football match on a live streaming app.

Missing a few frames is okay.
But if the stream lags, you miss the **goal moment**.
Real-time experience matters more than perfect accuracy.

**UDP is used** because it’s fast and supports real-time playback.

---
