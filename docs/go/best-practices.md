
- https://blog.codeship.com/utilizing-simplicity-go-easy-development/


Monorepo:
  - http://blog.shippable.com/our-journey-to-microservices-and-a-mono-repository
  - https://github.com/Shippable/support/issues/2640
    We have built a wrapper around the CI process that runs CI for different parts of the repo depending on what folders are changing.
    We have a root folder called _global, that if changes will trigger the whole system to be tested.
    Any local folder, will just trigger that folders CI.
  - https://www.meetup.com/go-toronto/events/229845521/


Web APIs:
- [Patterns and Examples for Building a Go Web App - Beyang Liu - 2014](https://www.youtube.com/watch?v=7zYXhhrRn2E)


Money:
  - https://github.com/shopspring/decimal

Common Mistakes:
  http://spf13.com/presentation/7-common-mistakes-in-go-2015/

Regex Testing:
  https://regex-golang.appspot.com/assets/html/index.html