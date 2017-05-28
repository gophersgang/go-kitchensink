### Concurrency Patterns


- [Go Concurrency Patterns - slides](https://present.go-steel-programmers.org/real_world_concurrency/2013-04-25.slide#5)
- [Go padawan - Concurrency Links](https://gopadawan.wordpress.com/recursos-sobre-go/)
- [Streams in Go- Firebase client](https://github.com/BlueMasters/firebasedb)
- [LearnConcurrency · golang/go Wiki](https://github.com/golang/go/wiki/LearnConcurrency) - really good!

- [How Goroutines Work](http://blog.nindalf.com/how-goroutines-work/)
- [Chapter 9. Concurrency with Shared Variables - Shichao's Notes](https://notes.shichao.io/gopl/ch9/)
- https://github.com/DiSiqueira/GoCurrency/blob/master/README.md
- [Parallel processing with ordered output in Go](https://gist.github.com/MarianoGappa/a50c4a8a302b8378c08c4b0d947f0a33)
- [Pipeline Processing - 2011/10](https://groups.google.com/forum/m/#!topic/golang-nuts/cHvGb_wOExw)
- [Pipelines in Golang - 2014/06](http://www.aktau.be/draft/2014/07/13/pipelines-in-golang/)
- [Gofragments - Concurrency](http://www.gofragments.net/concurrency)
- [Run strikingly fast parallel file searches in Go with sync.ErrGroup - 2016/09](https://www.oreilly.com/learning/run-strikingly-fast-parallel-file-searches-in-go-with-sync-errgroup)

- [SF - Feb 13 - Hangout with Patrick Crosby from Stathat and Phil Pennock from Apcera  - Go Concurrency in Production](https://www.youtube.com/watch?v=ruw0uOC4_Xk)

- [Principles of designing Go APIs with channels - 2014/08](https://inconshreveable.com/07-08-2014/principles-of-designing-go-apis-with-channels/)

## Concurrency with locks / Mutexes
  - [Dancing with Go’s Mutexes - 2015/11](https://medium.com/@deckarep/dancing-with-go-s-mutexes-92407ae927bf#.sht1rrymc)
  - https://www.cs.princeton.edu/courses/archive/fall16/cos418/docs/P1-concurrency.pdf (part of
    https://www.cs.princeton.edu/courses/archive/fall16/cos418/syllabus.html - Fall 2016: Distributed Systems)
  - https://blog.ksub.org/bytes/2015/10/11/the-little-go-book-of-semaphores/
  - http://whipperstacker.com/2015/10/05/3-trivial-concurrency-exercises-for-the-confused-newbie-gopher/
  - https://divan.github.io/posts/go_concurrency_visualize/ (FANTASTIC!)
  - https://www.oreilly.com/learning/run-strikingly-fast-parallel-file-searches-in-go-with-sync-errgroup
  - https://blog.golang.org/pipelines
  - https://kylewbanks.com/blog/tutorial-synchronizing-state-with-mutexes-golang
  - http://blog.rh-flow.de/2016/01/19/parallel-processing-of-csv-in-elixir-and-golang/
  - https://endophage.com/articles/golang-concurrency-patterns/
  - https://sharbeargle.gitbooks.io/golang-notes/content/master-worker-pattern.html
  - http://nesv.github.io/golang/2014/02/25/worker-queues-in-go.html


### Channels:
  - http://www.tapirgames.com/blog/golang-channel-closing
  - https://medium.com/stupid-gopher-tricks/more-powerful-synchronization-in-go-using-channels-f4a1c3242ed0#.1qnm8tqvq
  - https://inconshreveable.com/07-08-2014/principles-of-designing-go-apis-with-channels/
  - https://kylewbanks.com/blog/tutorial-synchronizing-state-with-mutexes-golang
  - http://dmitryvorobev.blogspot.de/2016/08/golang-channels-implementation.html
  - https://dave.cheney.net/2015/08/08/performance-without-the-event-loop

### Courses:
  - [Fundamentals of concurrent programming - 2014](http://www.nada.kth.se/~snilsson/concurrency/)
  - [GO, Concurrent&Systems Programming - 2012](https://www.cs.rit.edu/~ats/go-2011-2/index.xml)

### Videos (chronologically sorted)
  - https://github.com/arschles/go-in-5-minutes/issues/14
  - https://www.goin5minutes.com/screencast/episode_10_concurrency_the_daily_walk/
  - https://www.goin5minutes.com/screencast/episode_15_internet_cafe/
  - https://www.goin5minutes.com/screencast/episode_12_concurrency_eating_tapas/

  - [GopherCon 2015: Richard Fliam - A Practical Guide to Preventing Deadlocks and Leaks in Go](https://www.youtube.com/watch?v=3EW1hZ8DVyw)
  - [GopherCon 2016: Ivan Danyliuk - Visualizing Concurrency in Go](https://www.youtube.com/watch?v=KyuFeiG3Y60)
  - [GopherCon 2016: Adrian Cockcroft Communicating Sequential Goroutines](https://www.youtube.com/watch?v=gO1qF19y6KQ)
  - [channel go (2017)](https://www.youtube.com/watch?v=Pu6oFMLlpaQ)
  - [Concurrency: goroutines and channels (2014)](https://www.youtube.com/watch?v=zbFDjCHzN50)
  - [Google I/O 2013 - Advanced Go Concurrency Patterns](https://www.youtube.com/watch?v=QDDwwePbDtw)
  - [Google I/O 2012 - Go Concurrency Patterns](https://www.youtube.com/watch?v=f6kdp27TYZs)
  - [Golang Concurrency (2015/11)](https://www.youtube.com/watch?v=UP8agyrTeok&t=181s)


### Critical
  - https://mail.mozilla.org/pipermail/heka/2016-May/001059.html - [heka] State and future of Heka - why channels might complicate solution...
    - First, they don't perform well enough.
    - Second, they make it very hard to prevent message loss.
    - Third, the buffered channels mean that Heka consumes much more RAM than
would be otherwise needed,

    ====>>> solution: Hindsight avoids all of these problems by using disk queues instead of
RAM buffers between all of the processing stages.


