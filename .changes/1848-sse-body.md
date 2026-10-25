### Fixed

- **`@reticlehq/browser` — capture streamed SSE replies.** With network body capture on, Reticle now records `text/event-stream` responses without blocking the app or delaying settle. Capture stops at its size bound or after 10 seconds. JSON event data uses structured credential redaction. Incomplete bodies carry a truncation flag, so missing text returns `unknown`, not `no`. Closes [#1848](https://github.com/reticlehq/reticle/issues/1848).
