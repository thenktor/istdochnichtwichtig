# istdochnichtwichtig

A minimal blogging theme for Hugo that respects your privacy and is easy on your bandwidth.

A real-life example can be found at [](https://www.gebiert.de).

istdochnichtwichtig is based on [smol](https://github.com/colorchestra/smol) created by [morph](https://morph.sh/).


## Features

- No JavaScript
- No Google spyware or tracking of any kind
- No other external dependencies, external fonts or comment sections
- Dark mode support (depending on your OS's setting)

## Installation

In your Hugo site `themes` directory, run:

```
git clone https://github.com/thenktor/istdochnichtwichtig
```

Next, open `config.toml` in the base of the Hugo site and ensure the theme option is set to `istdochnichtwichtig`.

```
theme = "istdochnichtwichtig"
```

You can also add the following to `config.toml`

```
[params]
description = "Here is the description of the web site"
subtitle = "Bier trinken ist wichtig!"

# web site logo besides title
logo = "/logo.png"

# favicon
favicon = "/favicon.png"
# as png instead of ico
faviconType = "image/png"

# Apple touch icon
appleTouchIcon = "/apple-touch-icon.png"

# custom CSS files
customCSS = ["css/custom.css"]

# how many antries should the list have? (tags, categories, ...)
paginateList = 100
```

Lastly, add the following lines to your `config.toml` to make use of all the menu entries in the header and footer sections if you need them.

```
# Header
[menu]
  [[menu.main]]
        identifier = "posts"
        name = "Posts"
        url = "/posts/"
        weight = 1 

  [[menu.main]]
        identifier = "categories"
        name = "Categories"
        url = "/categories/"
        weight = 2 

  [[menu.main]]
        identifier = "tags"
        name = "Tags"
        url = "/tags/"
        weight = 3

# Footer
  [[menu.footer]]
        name = "Github"
        url = "https://github.com/example"
        weight = 1 

    [[menu.footer]]
        name = "Privacy"
        url = "/privacy"
        weight = 2 

    [[menu.footer]]
        name = "Imprint"
        url = "/imprint"
        weight = 3 

```

For more information read the official [quick start guide](https://gohugo.io/getting-started/quick-start/) of Hugo.

## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/thenktor/istdochnichtwichtig/issues) to let me know. Or make directly a [pull request](https://github.com/thenktor/istdochnichtwichtig/pulls).

## License

This theme is released under the [MIT license](https://github.com/thenktor/istdochnichtwichtig/blob/master/LICENSE).
