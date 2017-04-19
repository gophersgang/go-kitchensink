### Monorepo:


- https://twitter.com/hashtag/monorepo?src=hash
- https://dzone.com/articles/monolithic-repositories-more-pros-than-cons
- https://trunkbaseddevelopment.com/monorepos/


### Trunk based Development

  - https://trunkbaseddevelopment.com/
  - [Google's vs Facebook's Trunk Based Development](http://paulhammant.com/2014/01/08/googles-vs-facebooks-trunk-based-development/) - great points!
  - http://blog.plasticscm.com/2017/04/how-we-do-trunk-based-development-with.html
  - https://paulhammant.com/2017/02/14/pre-commit-continuous-integration-infrastructure-is-cheaper-than-post-commit-for-high-throughput-teams/
  - http://www.gigamonkeys.com/flowers/


### Videos:
  - [Uber Technology Day: Monorepo to Multirepo and Back Again - 2017/04](https://www.youtube.com/watch?v=lV8-1S28ycM)
  - https://speakerdeck.com/kageiit/lightning-fast-android-builds-with-gradle-plus-buck
  - [Python Pants - A build system for large codebases with multiple dependencies - PyConSG 2016](https://www.youtube.com/watch?v=Q6sLN8rqkDE&t=1s)
  - [Building Software at Google Scale: Bazel](https://www.youtube.com/watch?v=6GCDfoAOKIY)
  - [Bazel: Google's own build tool, now publicly available in Beta by Paul Johnston - 2016/12](https://www.youtube.com/watch?v=G-4jqDgILCM)
  - [The Pants Build Tool at Twitter - 2014](https://www.youtube.com/watch?v=j_4CVpOIWsE)


## Javascript
  - https://github.com/guigrpa/oao


#### Software
  - https://github.com/Originate/morula - task runner for monorepos
  - https://speakerdeck.com/fabpot/a-monorepo-vs-manyrepos
  -


#### Articles
  - [FASTER TOGETHER: UBER ENGINEERING’S IOS MONOREPO - 2017/04](https://eng.uber.com/ios-monorepo/)
  - [3.5 Years, 500k Lines of Go (Part 1) - 2017/03](https://npf.io/2017/03/3.5yrs-500k-lines-of-go/)

  - [Tech In Asia Monorepo move - 2016/12](https://www.techinasia.com/talk/tia-engineering-monorepo-move)
  - https://speakerdeck.com/sergeyz/a-monorepo-vs-manyrepos-the-oro-way

  - [Dropbox - Comment on Go code in on repo](https://youtu.be/JOx9enktnUM?t=1113)
    - 400k non-generated Go code
    - 130 contributors
    - all infrastructure in go
    - all new things in go.

  - https://storify.com/samnewman/in-which-i-discuss-monorepos (2017/03)
  - http://www.drmaciver.com/2016/10/why-you-should-use-a-single-repository-for-all-your-companys-projects/

  - [Digital Ocean - Bryan Liles - Go At Work](https://youtu.be/Kx0nUrTItR0?t=958)
  - http://dev.pumpup.com/post/reducing-android-build-times-with-buck#library-build-rules


  - [Why is Babel a monorepo? - 2016](https://github.com/babel/babel/blob/master/doc/design/monorepo.md)
  - [Why We Should Use Monolithic Repositories](https://gist.github.com/arschles/5d7ba90495eb50fa04fc)
  - [Go in a Monorepo - 2015 (digital ocean)](https://blog.gopheracademy.com/advent-2015/go-in-a-monorepo/)
  - [On Monolithic Repositories - 2014](http://gregoryszorc.com/blog/2014/09/09/on-monolithic-repositories/)

  - https://cacm.acm.org/magazines/2016/7/204032-why-google-stores-billions-of-lines-of-code-in-a-single-repository/fulltext
  - [Taming Your Go Dependencies - 2015/02](https://www.digitalocean.com/company/blog/taming-your-go-dependencies/)
  - http://blog.shippable.com/our-journey-to-microservices-and-a-mono-repository
  - https://github.com/Shippable/support/issues/2640
    We have built a wrapper around the CI process that runs CI for different parts of the repo depending on what folders are changing.
    We have a root folder called _global, that if changes will trigger the whole system to be tested.
    Any local folder, will just trigger that folders CI.
  - https://www.meetup.com/go-toronto/events/229845521/


  - http://blog.traintracks.io/monorepo-shared-code-and-isolated-fast-docker-builds

  - [Staffjoy’s V2 Architecture](https://blog.staffjoy.com/staffjoys-v2-architecture-9d2fcb4015fd#.z8fydno1x)
    - https://github.com/Staffjoy/v2

  philip1209:
    Yes. I would always use gRPC-gateway in the future. It's an amazing library. Check out the `protobuf` folder - we basically defined the whole api there in a language-agnostic way. For client libraries, you can autogenerate gRPC definitions quickly. For servers, gRPC-gateway provides a Swagger definition that meant that we always had 100% up to date API docs that include a Postman-style way to execute calls. The auto-generated API docs sped up front-end development so much.
    I think that access to the docs requires logging in, so here are some screenshots: http://imgur.com/a/R0AvB
    Jason Chen is using Elixer/Phoenix for his new project, by the way, and thinks that it's the future for Rails developers.

    ...
    Yes. Protocol buffers and grpc-gateway made it easy to scaffold out a quick api, write all the interior logic, and know that there would not be any major issues due to strong typing. We used Gogoproto to annotate the protobuf files so that database crud is easy too.

    ...
    I'm already starting on my next company. It's a monorepo with three folders: pkg (packages), cmd (any `package main` commands), and static (all JS, SCSS, etc that gets built by Webpack then wrapped up in a single bindata.go). The primary app is a monolith. However, I'm making it possible to add additional service, such as cron jobs in separate containers or a command line utility based on the same protobuf definition.

    ...
    The Bazel build system [1] is the open-source version of Google's internal build system. It's tough to set up, but once you do - it caches all builds, down to the docker container generation. On changes, it analyzes affected upstream projects and selectively rebuilds them. So, after an initial build, rebuilds are blazingly fast. In fact, the simple act of creating a pull request means that most production builds/deploys come straight from cache.
    Here [2] is a screenshot of the actual "master branch test, lint, build, and deploy 15 containers to kubernetes" job from our Jenkins. It took about 10 minutes on the build box every time.
    That being said, in order to make builds work with Bazel, we had to do some wonky stuff. We committed built Javascript files, and we had to manually commit a lot of other types of data files (like bindata.go and protobuf outputs).



### Pants
  - [Smarty Pants: Improving our Python Build - 2015/11](http://oscardna.tumblr.com/post/133010618340/smartypants)


### Bazel
  - https://github.com/google/nomulus (real example)
  - https://github.com/laramiel/bazel-example-golang
  - https://github.com/bazelbuild/bazel
  - https://www.kchodorow.com/blog/2015/12/08/combining-projects-without-converting-to-a-monorepo/
  - http://isilmar-4.linta.de/~aehlig/university/slides/conf/fosdem17.pdf

### Buck
  - https://news.ycombinator.com/item?id=13865400 (2017/02)
  - [Basics: Building with Buck - 2016/11](https://www.youtube.com/watch?v=sZdDFfNJeuU)


### Big repos
  - https://news.ycombinator.com/item?id=7648237 -  Facebook's git repo is 54GB


### Tooling / Code Review
  - Phabricator:
    - https://news.ycombinator.com/item?id=12487695
    - Phabricator is a really solid GitHub alternative. Some of the largest open source projects are using it and lots of companies.


    - https://dzone.com/articles/the-13-things-that-make-a-good-build-system


### companies
  - https://blog.ngzhian.com/three-internships.html


### Monorepos in general

  - https://www.reddit.com/r/programming/comments/42gx7v/advantages_of_monolithic_version_control/
  - https://blog.ghaering.de/post/monorepo-march/
  - https://blog.asana.com/2015/09/sane-build-systems/
