# wildmatch

[![](https://docs.rs/wildmatch/badge.svg)](https://docs.rs/wildmatch)
[![](http://meritbadge.herokuapp.com/wildmatch)](https://crates.io/crates/wildmatch)
[![](https://badgen.net/crates/d/wildmatch)](https://crates.io/crates/wildmatch)
[![Build Status](https://gitlab.com/becheran/wildmatch_ci/badges/master/pipeline.svg)](https://gitlab.com/becheran/wildmatch_ci/pipelines)
[![](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Codecov branch](https://img.shields.io/codecov/c/github/becheran/wildmatch/master)](https://codecov.io/gh/becheran/wildmatch)

Match strings against a simple wildcard pattern. Tests a wildcard pattern `p` against an input string `s`. Returns true only when `p` matches the entirety of `s`.

See also the example described on [wikipedia](https://en.wikipedia.org/wiki/Matching_wildcards) for matching wildcards.

- `?` matches exactly one occurrence of any character.
- `*` matches arbitrary many (including zero) occurrences of any character.
- No escape characters are defined.

For example the pattern `ca?` will match `cat` or `car`. The pattern `https://*` will match all https urls, such as `https://google.de` or `https://github.com/becheran/wildmatch`.

The library only depends on the rust [`stdlib`](https://doc.rust-lang.org/std/).

See the [documentation](https://docs.rs/wildmatch) for usage and more examples.
