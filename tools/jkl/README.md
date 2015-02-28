# **jkl** is a static site generator

Written in [Go](http://www.golang.org), based on [Jekyll](https://github.com/mojombo/jekyll)

Notable similarities between jkl and Jekyll:

* Directory structure
* Use of YAML front matter in Pages and Posts
* Availability of `site`, `content`, `page` and `posts` variables in templates
* Copies all static files into destination directory

Notable differences between jkl and Jekyll:

* Uses [Go templates](http://www.golang.org/pkg/text/template)
* Only supports YAML front matter in markup files
* No plugin support

Sites built with jkl:

* Drone.io Blog: http://blog.drone.io
* Drone.io Documentation: http://docs.drone.io

--------------------------------------------------------------------------------

### Installation

```
go get github.com/golang-china/golang-china.github.com/tools/jkl
```

### Usage

```
Usage: jkl [OPTION]... [SOURCE]

      --auto           re-generates the site when files are modified
      --base-url       serve website from a given base URL
      --source         changes the dir where Jekyll will look to transform files
      --destination    changes the dir where Jekyll will write files to
      --server         starts a server that will host your _site directory
      --server-port    changes the port that the Jekyll server will run on
  -v, --verbose        runs Jekyll with verbose output
  -h, --help           display this help and exit

Examples:
  jkl                  generates site from current working dir
  jkl --server         generates site and serves at localhost:4000
  jkl /path/to/site    generates site from source dir /path/to/site

```

### Auto Generation

If you are running the website in server mode, with the `--server` flag, you can
also instruct `jkl` to auto-recompile you website by adding the `--auto` flag.

NOTE: this feature is only available on Linux


### Documentation

See the official [Jekyll wiki](https://github.com/mojombo/jekyll/wiki)
... just remember that you are using Go templates instead of Liquid templates.

