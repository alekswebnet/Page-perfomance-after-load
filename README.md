# Page perfomance after load
Web performance optimization tips from Google Chrome Developers ([video on YouTube](//www.youtube.com/watch?v=4QkuvwRftTw))

## 📐 Measure first

### Measure real data

* the lab is one config out of millions
* lab data can give false confidence
* gather **real** data from **real** users
* send to your analytics

More - [web.dev/vitals-field-measurement-best-practices/](//web.dev/vitals-field-measurement-best-practices/).

## ⏳ Free up the main thread

***Free main thread means smoothness is governed primarily by layout***

### Web Worker

* offload heavy lifting to a Worker
* good for parsers, formatters, validation, number crunching

### Paint Worklet

* move canvas-based graphics off the main thread
* build-in caching and batching
* draw based on layout geometry, without forcing layout

Check out [houdini.how](//houdini.how) for reusable worklets.

## 🧹 Minimaze memory usage

***Smoothness and responsiveness can be affected by memory usage***

### Memory usage

* avoid excessive memort usage
* consider where to cache
* monitor for memory leaks

More - [web.dev/detached-window-memory-leaks/](//web.dev/detached-window-memory-leaks/)

## ✔️ Load with best-practices

### Best-practices for loading still apply

* **code-split** JS to load as-needed
* **preload** in idle time
* **defer** invisible content
* **lazy-load** embeds
* **avoid inlining** assets into JS

## ⚡ Ship modern code

### Ship fast, modern code

* transpile for 90% case
* modern code is fast
* avoid automatic polyfilling
* serve legacy code via nomodule

More - [web.dev/publish-modern-javascript/](//web.dev/publish-modern-javascript/)
