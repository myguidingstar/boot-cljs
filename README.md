# boot-cljs-alt

Proof of concept. Minimal ClojureScript task for Boot.

Running [ClojureScript directly](https://github.com/clojure/clojurescript/wiki/Reporting-Issues)
is surprisingly easy and works really well. I created this task to test
how well minimal ClojureScript task would work.

## Differences to boot-cljs

- Uses fewer tempdirs

| Boot-cljs | *This*
--- | --- | ---
Lines of code | 396 | 45
--- | --- | ---
Cold build time | 9.5s | 9.5s
Watch build time | 0.25s | 0.25s

Tested with [saapas][saapas]

## Results

- No performance improvements despite using fewer tempdirs, at least on Linux

## Missing features

- [ ] Setting `:main` and `:output-to` from `.cljs.edn`
- [ ] Error reporting
- [ ] [boot-reload][boot-reload] support.

## License

Copyright © 2014 Adzerk
Copyright © 2015 Juho Teperi

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.

[boot-cljs]: https://github.com/adzerk-oss/boot-cljs
[boot-reload]: https://github.com/adzerk-oss/boot-reload
[saapas]: https://github.com/Deraen/saapas
