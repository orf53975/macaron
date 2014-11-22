Macaron [![Build Status](https://drone.io/github.com/Unknwon/macaron/status.png)](https://drone.io/github.com/Unknwon/macaron/latest) [![](http://gocover.io/_badge/github.com/Unknwon/macaron)](http://gocover.io/github.com/Unknwon/macaron)
=======================

![Macaron Logo](macaronlogo.png)

Package macaron is a high productive and modular design web framework in Go.

##### Current version: 0.4.3

## Getting Started

To install Macaron:

	go get github.com/Unknwon/macaron

The very basic usage of Macaron:

```go
package main

import "github.com/Unknwon/macaron"

func main() {
	m := macaron.Classic()
	m.Get("/", func() string {
		return "Hello world!"
	})
	m.Run()
}
```

## Features

- Powerful routing with suburl.
- Flexible routes combinations.
- Unlimited nested group routers.
- Directly integrate with existing services.
- Dynamically change template files at runtime.
- Easy to plugin/unplugin features with modular design.
- Handy dependency injection powered by [inject](https://github.com/codegangsta/inject).
- Better router layer and less reflection make faster speed.

## Middlewares 

Middlewares allow you easily plugin/unplugin features for your Macaron applications.

There are already many [middlewares](https://github.com/macaron-contrib) to simplify your work:

- [binding](https://github.com/macaron-contrib/binding) - Request data binding and validation
- [i18n](https://github.com/macaron-contrib/i18n) - Internationalization and Localization
- [cache](https://github.com/macaron-contrib/cache) - Cache manager
- [session](https://github.com/macaron-contrib/session) - Session manager
- [csrf](https://github.com/macaron-contrib/csrf) - Generates and validates csrf tokens
- [captcha](https://github.com/macaron-contrib/captcha) - Captcha service
- [pongo2](https://github.com/macaron-contrib/pongo2) - Pongo2 template engine support
- [sockets](https://github.com/macaron-contrib/sockets) - WebSockets channels binding
- [toolbox](https://github.com/macaron-contrib/toolbox) - Health check, pprof, profile and statistic services
- [switcher](https://github.com/macaron-contrib/switcher) - Multiple-site support
- [renders](https://github.com/macaron-contrib/renders) - Beego-like render engine(Macaron has built-in template engine, this is another option)

## Use Cases

- [Gogs](https://github.com/gogits/gogs): Go Git Service
- [Gogs Web](https://github.com/gogits/gogsweb): Gogs official website
- [Switch](https://github.com/gpmgo/switch): Gopm registry
- [YouGam](http://yougam.com): Online Forum
- [Car Girl](http://qcnl.gzsy.com/): Online campaign

## Getting Help

- [API Reference](https://gowalker.org/github.com/Unknwon/macaron)
- [Documentation](http://macaron.gogs.io)
- [FAQs](http://macaron.gogs.io/docs/faqs)

## Credits

- Basic design of [Martini](https://github.com/go-martini/martini).
- Router layer of [beego](https://github.com/astaxie/beego).
- Logo is modified by [@insionng](https://github.com/insionng) based on [Tribal Dragon](http://xtremeyamazaki.deviantart.com/art/Tribal-Dragon-27005087).

## License

This project is under Apache v2 License. See the [LICENSE](LICENSE) file for the full license text.