# [Bisect_ppx][bisect] + Js_of_ocaml starter repo

```
git clone https://github.com/aantron/bisect-starter-jsoo.git
cd bisect-starter-jsoo
opam install -y --deps-only .
BISECT_ENABLE=yes dune build ./tester.bc.js
node _build/default/tester.bc.js
dune exec bisect-ppx-report -- --html _coverage/ *.out
```

These commands generate
[this coverage report](https://aantron.github.io/bisect-starter-jsoo/) locally
in the `_coverage/` directory. Use your browser to open `_coverage/index.html`!

[Here][demo] is an example of a coverage report for a real-world project.

See [aantron/bisect_ppx][bisect], especially the
[Js_of_ocaml instructions][jsoo-instructions].

[bisect]: https://github.com/aantron/bisect_ppx
[jsoo-instructions]: https://github.com/aantron/bisect_ppx#Js_of_ocaml
[demo]: https://aantron.github.io/bisect_ppx/demo/
