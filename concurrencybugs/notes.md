# Concurrency Bugs In Go

### A tour of all the ways concurrency can bite you, and how to avoid them

* shadowed variables in goroutine for loop

* non blocking send with chan read in goroutine https://play.golang.org/p/IUIExsK9mKf fix by buffering channel

* waitgroup add inside goroutine

* cyclical work channels can lead to deadlock https://play.golang.org/p/6DMOUURV6pu

## Key Takeaways
* the 'go' keyword is a wormhole, you don't know where/when this code will execute
