We use [pack](https://github.com/stefan-hoeck/idris2-pack) to organise our projects. Put the following in `~/.pack/user/pack.toml` to use the most recent package versions:

```
[custom.all.log-domain]
type   = "github"
url    = "https://github.com/idris-bayes/log-domain"
commit = "latest:master"
ipkg   = "log-domain.ipkg"

[custom.all.distributions]
type   = "github"
url    = "https://github.com/idris-bayes/distributions"
commit = "latest:master"
ipkg   = "distributions.ipkg"

[custom.all.free]
type   = "github"
url    = "https://github.com/idris-bayes/free"
commit = "latest:master"
ipkg   = "free.ipkg"

[custom.all.monad-bayes]
type   = "github"
url    = "https://github.com/idris-bayes/monad-bayes"
commit = "latest:master"
ipkg   = "monad-bayes.ipkg"

[custom.all.prob-fx]
type   = "github"
url    = "https://github.com/idris-bayes/prob-fx"
commit = "latest:master"
ipkg   = "prob-fx.ipkg"
```

Note that many of these projects will interface with C shared object files (`.so` files) which are included locally in their repositories. Currently, other projects that depend on them will also need to have their `.so` files locally.
