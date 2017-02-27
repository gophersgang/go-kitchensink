### Monorepo:

  - [Why We Should Use Monolithic Repositories](https://gist.github.com/arschles/5d7ba90495eb50fa04fc)
  - [Go in a Monorepo - 2015 (digital ocean)](https://blog.gopheracademy.com/advent-2015/go-in-a-monorepo/)
  - [Taming Your Go Dependencies - 2015/02](https://www.digitalocean.com/company/blog/taming-your-go-dependencies/)
  - http://blog.shippable.com/our-journey-to-microservices-and-a-mono-repository
  - https://github.com/Shippable/support/issues/2640
    We have built a wrapper around the CI process that runs CI for different parts of the repo depending on what folders are changing.
    We have a root folder called _global, that if changes will trigger the whole system to be tested.
    Any local folder, will just trigger that folders CI.
  - https://www.meetup.com/go-toronto/events/229845521/
