Patterns:
  - http://www.alexedwards.net/blog/organising-database-access
  - https://www.vividcortex.com/blog/2015/09/22/common-pitfalls-go/
  - https://www.reddit.com/r/golang/comments/5vsz2t/what_is_the_best_way_to_pass_a_db_to_web_handlers/

Tutorials
  - http://go-database-sql.org/index.html


Query builder:
  - https://github.com/Masterminds/squirrel (active)
  - https://github.com/doug-martin/goqu (active)
  - https://github.com/shuoli84/sqlm (really minimal)
  - https://github.com/fragmenta/query (also quite minimal)
  - https://github.com/umisama/go-sqlbuilder

ORM:
  - https://github.com/mgutz/dat (JUST FOR Postgres, but good!)
  - https://github.com/go-gorp/gorp (not really maintained...)
  - https://github.com/go-xorm (looks really ok, used in some projects, chinese)

  - https://github.com/markbates/pop (newcomer, from gobuffalo)

Static Generators:
  - https://github.com/vattle/sqlboiler

Query generator: (static, but looks quite interesting...)
- https://github.com/vattle/sqlboiler#a-small-taste


Map Templates to queries:
  - https://github.com/gchaincl/dotsql

Simple libs:
  - https://github.com/jmoiron/sqlx

Db mapper:
  - https://github.com/upper/db
  - https://github.com/Masterminds/structable


Repository Pattern in Go:
  - http://docs.basho.com/riak/kv/2.2.0/developing/getting-started/golang/object-modeling/ (great examples!)
  - https://www.youtube.com/watch?v=wB1hoUJDbk0 (TaskManager (like Repo))
  - http://matthewbrown.io/2016/01/23/factory-pattern-in-golang/
  - http://docs.basho.com/riak/kv/2.2.0/developing/getting-started/golang/object-modeling/

DB testing:
  - https://github.com/DATA-DOG/go-sqlmock

Migration:
  - https://povilasv.me/2017/02/20/go-schema-migration-tools/
  - http://slides.com/gchaincl/select-golang-from-languages
  - https://github.com/pressly/goose


Slides:
  - http://slides.com/akshaydeo/writing-web-apps-in-golang/embed
  - http://blog.carbonfive.com/2015/07/09/there-will-be-sql/
  - https://www.reddit.com/r/golang/comments/5vbv7u/golang_web_dev_frameworks/

### Intros:
  - https://hackernoon.com/how-to-work-with-databases-in-golang-33b002aa8c47#.n57nc6x12

### Migrations:
    - https://github.com/mattes/migrate (has quite a lot dependencies)
    - https://github.com/DavidHuie/gomigrate (much less features, but no hard dependencies)
    - http://www.sivachandran.in/2016/04/embedding-db-migrations-through-golang.html

### ORM
    - https://www.reddit.com/r/golang/comments/3ajqa6/golang_which_orm_is_better/
        - https://github.com/mgutz/dat
        - https://github.com/jmoiron/sqlx
        - https://github.com/vattle/sqlboiler (fast and simple (aka generated))
        - https://github.com/go-gorp/gorp ()

### Fixtures:
  - https://github.com/theplant/gofixtures
