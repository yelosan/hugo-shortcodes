# Shortcodes for Hugo

A collection of custom shortcodes used in [YourOnly.One](https://YourOnly.One) and other Hugo-powered websites made by YourOnly.One.

## Repository, suggestions, issues, pull requests

We use [Codeberg](https://codeberg.org/yelosan/hugo-shortcodes) for development, suggestions, issues, and pull requests.

### Mirrors

- [GitHub](https://github.com/yelosan/hugo-shortcodes), original home.
- [GitLab](https://gitlab.com/yelosan/hugo-shortcodes), second home.

> *Note:* These mirrors should not be used as a Hugo module as it will produce a GoLang module error. The `go.mod` ID is set to `codeberg.org/yelosan/hugo-shortcodes` which should match the URL Hugo/GoLang is fetching it from.

## Installation

Installation is being re-worked.

### Customise the shortcodes

If you want to customise the shortcodes in this git, the advisable method is the following:

1. Copy `your-hugo-project/themes/hugo-shortcodes/layouts/shortcodes/{shortcode}.html` to `your-hugo-project/layouts/shortcodes/{shortcode}.html`
2. Edit your own copy of `{shortcode}.html`
    - Hugo will always use your copy of `{shortcode}.html`.

## Shortcodes

- `{{< image >}}`

- `{{< music >}}`
- `{{% quotebox %}}`
- `{{< scribd >}}`
- `{{< youtube >}}`
