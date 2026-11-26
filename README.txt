QR Beam (prototype)
==================

This is a starter optical QR transfer prototype, not a complete Decimen clone.

Open index.html in a modern browser. Camera scanning may require a secure context
(HTTPS or localhost). The QR library and scanner are loaded from CDN, so the
app requires internet to load those libraries initially.

Prototype limitations:
- 2 MB file size limit
- Simple repeated QR chunks, no fountain coding/error correction across missing frames
- Receiver needs to capture all chunks; sender repeats frames
- For robust, large files and offline operation, vendor the JS libraries and implement
  fountain coding (e.g. robust soliton / LT codes) and a frame protocol.

