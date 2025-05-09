This fork just removes couple of lines which makes Ebitenmobile able to compile Android builds on non-Darwin arm64 environments, especially prooted Debian on Termux which is what i use, but this should work on other arm64 environments.

To be able to compile, set the `EBITENMOBILE_GOMOBILE` environment variable to your local copy of this repo. (Example: `EBITENMOBILE_GOMOBILE=/root/gomobile ebitenmobile`, when in a prooted environment)

# Go support for Mobile devices

[![Go Reference](https://pkg.go.dev/badge/github.com/ebitengine/gomobile.svg)](https://pkg.go.dev/github.com/ebitengine/gomobile)

The Go mobile repository holds packages and build tools for using Go on mobile platforms.

Package documentation as a starting point:

- [Building all-Go apps](https://github.com/ebitengine/gomobile/app)
- [Building libraries for SDK apps](https://github.com/ebitengine/gomobile/cmd/gobind)

![Caution image](doc/caution.png)

The Go Mobile project is experimental. Use this at your own risk.
While we are working hard to improve it, neither Google nor the Go
team can provide end-user support.

This is early work and installing the build system requires Go 1.5.
Follow the instructions on
[golang.org/wiki/Mobile](https://golang.org/wiki/Mobile)
to install the gomobile command, build the
[basic](https://github.com/ebitengine/gomobile/example/basic)
and the [bind](https://github.com/ebitengine/gomobile/example/bind) example apps.

--

Contributions to Go are appreciated. See https://go.dev/doc/contribute.

The git repository is https://go.googlesource.com/mobile.

* Bugs can be filed at the [Go issue tracker](https://go.dev/issue/new?title=x/mobile:+).
* Feature requests should preliminary be discussed on
[golang-nuts](https://groups.google.com/forum/#!forum/golang-nuts)
mailing list.
