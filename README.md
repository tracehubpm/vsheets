[![EO principles respected here](https://www.elegantobjects.org/badge.svg)](https://www.elegantobjects.org)
[![DevOps By Rultor.com](http://www.rultor.com/b/trarcehubpm/vsheets)](http://www.rultor.com/p/tracehubpm/vsheets)
[![We recommend IntelliJ IDEA](https://www.elegantobjects.org/intellij-idea.svg)](https://www.jetbrains.com/idea/)

[![rake](https://github.com/tracehubpm/vsheets/actions/workflows/rake.yml/badge.svg)](https://github.com/tracehubpm/vsheets/actions/workflows/rake.yml)
[![Hits-of-Code](https://hitsofcode.com/github/tracehubpm/vsheets)](https://hitsofcode.com/view/github/tracehubpm/vsheets)
[![PDD status](http://www.0pdd.com/svg?name=tracehubpm/vsheets)](http://www.0pdd.com/p?name=tracehubpm/vsheets)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/tracehubpm/vsheets/blob/master/LICENSE.txt)

Validation XSL sheets for project artifacts.

### Sheets

XSL sheets are located inside `xsl` directory.

All of them will be fetched by @tracehubgit to validate quality
of artifacts in your project, it includes:
* Jobs
* Artifacts
* Team structure
* TBD..

Each sheet must have a unit tests.
We are keeping them inside [spec](https://github.com/tracehubpm/vsheets/tree/master/spec).

For instance, take a look at [`struct.xsl`](https://github.com/tracehubpm/vsheets/blob/master/xsl/struct.xsl) 
and [`struct_spec.rb`](https://github.com/tracehubpm/vsheets/blob/master/spec/struct_spec.rb).

### How to contribute?

First install [Ruby 3.1.4+](https://www.ruby-lang.org/en/news/2023/03/30/ruby-3-1-4-released)
and [Bundler](https://bundler.io).

Then run:

```
$ bundle update
$ bundle exec rake
```

The build has to be clean. If it's not, [submit an issue](https://github.com/tracehubpm/vsheets/issues).

Then, make your changes, make sure the build is still clean, and [submit a pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
