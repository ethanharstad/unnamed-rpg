# Website for unnamed rpg game

## Using

1. [Install Hugo](https://gohugo.io/overview/installing/)
2. Clone this repository
```bash
git clone git@github.com:ethanharstad/unnamed-rpg.git
cd unnamed-rpg
```
3. Run Hugo
```bash
hugo server
```

## Authoring

### Shortcodes

Several shortcodes have been added to make authoring easier

#### Alert

```markdown
{{< alert type="primary" title="A Note" >}}
Inner Text
{{< /alert >}}
```

`type` is an optional parameter and can be one of the following: `primary`, `secondary`, `success`, `danger`, `warning`, `info`, `light`, or `dark`.

`title` is an optional parameter that will set a title on the alert.

#### Link

```markdown
{{< link path="path" text="link text" >}}
```

`path` is the string path to a hugo page.
The page title will be used as the link text unless overridden.
If no text is provided, the `path=` portion can be omitted and provided as a bare string instead.

`text` is an optional parameter that overrides the link text.

## Behind the scenes

The site is built with [Hugo](https://gohugo.io) and [Bootstrap](https://getbootstrap.com/).

The site is hosted on [Cloudflare Pages](https://developers.cloudflare.com/pages/).

[Decap CMS](https://decapcms.org/) (formerly Netlify CMS) is used with a [custom auth gateway](https://github.com/i40west/netlify-cms-cloudflare-pages).
