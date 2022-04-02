# Shortcodes for [Hugo](https://gohugo.io)
A collection of custom shortcodes used in [YourOnly.One](https://YourOnly.One) and other Hugo-powered websites made by YourOnly.One.

## Setup
1. Add Hugo Shortcodes git in your Hugo project:
    * Method 1: git submodule
        ```shell
        cd your-hugo-project
        git submodule add https://github.com/techmagus/hugo-shortcodes.git themes/hugo-shortcodes
        ```
        * To update:
          ```shell
          cd your-hugo-project
          git submodule update --remote --merge themes/hugo-shortcodes
          ```

    * Method 2: git clone
        ```shell
        cd your-hugo-project
        git clone https://github.com/techmagus/hugo-shortcodes.git themes/hugo-shortcodes
        ```
        * To update:
          ```shell
          cd your-hugo-project/themes/hugo-shortcodes
          git pull
          ```
1. Add `hugo-shortcodes` in your project:

    `config.toml`:
    ```toml
    theme = ["hugo-shortcodes", "my-theme"]
    ```
    `config.yaml`:
    ```yaml
    theme:
      - hugo-shortcodes
      - my-theme
    ```

### Customise the shortcodes
If you want to customise the shortcodes in this git, the advisable method is the following:
1. Copy `your-hugo-project/themes/hugo-shortcodes/layouts/shortcodes/{shortcode}.html` to `your-hugo-project/layouts/shortcodes/{shortcode}.html`
2. Edit your own copy of `{shortcode}.html`
    * Hugo will always use your copy of `{shortcode}.html`.

## Shortcodes
* `{{< image >}}`
* `{{< instagram >}}`
* `{{< music >}}`
* `{{% quotebox %}}`
* `{{< scribd >}}`
* `{{< youtube >}}`

### How to use {{< image >}}
```go
{{< image
  type="image OR imagecoverattrib"

  imgheight=""
  imgwidth=""

  imgsrc=""
  imglink=""
  imgrel="noopener external nofollow"

  imgtitle="formal title"
  imgcaption="description"
  imgalt=""

  attribalign=""

  licensecode="any OR cc0 OR publicdomain OR allrightsreserved"
  licenseurl=""
  licensename=""

  attribto=""
  attriblink=""
  attribrel="noopener external nofollow"
>}}
```

### How to use {{< instagram >}}
```go
{{< instagram POST_ID hidecaption >}}
```

### How to use {{< music >}}
```go
{{< music src="" >}}
```

### How to use {{% quotebox %}}
```go
{{% quotebox boxstyle="qbs_generic" qmarkstyle="qbm_doublequotationmark" boxcolour="qbc_blue" attribalign="txt_right" srctitle="" srclink="" srcrel="noopener external nofollow" attribto="" attriblink="" attribrel="noopener external nofollow" %}}
  content
{{% /quotebox %}}
```

### How to use {{< scribd >}}
```go
{{< scribd
  doctitle=""
  docid=""
  startpage="1"
  viewmode="slideshow OR scroll"
  docrel="noopener external nofollow"

  authorname=""
  authorid=""
  authorrel="noopener external nofollow"
>}}
```

### How to use {{< youtube >}}
```go
{{< youtube id="" title="" >}}
```
