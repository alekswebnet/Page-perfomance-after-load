# Page perfomance after load
Web performance optimization tips from Google Chrome Developers

## Measure first

* the lab is one config out of millions
* lab data can give false confidence
* gather **real** data from **real** users
* send to your analytics

More - [web.dev/vitals-field-measurement-best-practices/](//web.dev/vitals-field-measurement-best-practices/).

## Free up the main thread

### Web Worker

* offload heavy lifting to a Worker
* good for parsers, formatters, validation, number crunching

### Paint Worklet

* move canvas-based graphics off the main thread
* build-in caching and batching
* draw based on layout geometry, without forcing layout

Check out [houdini.how](//houdini.how) for reusable worklets.

## Minimaze memory usage

## Load with best-practices

## Ship modern code
