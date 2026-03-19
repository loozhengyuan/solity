# `solity`

SDK for Solity Smart Lock.

## Development

### Docs

Documentation is generated using [Hugo](https://gohugo.io/) and deployed on [Cloudflare Pages](https://pages.cloudflare.com).

To preview documentation locally, you can use the `hugo` command:

```shell
hugo server --source ./docs --buildDrafts --disableFastRender
```

Certain logic (e.g. redirects) may require using the [`wrangler`](https://developers.cloudflare.com/workers/wrangler/) for preview instead:

```shell
wrangler pages dev --cwd ./docs
```

## License

[MIT](https://choosealicense.com/licenses/mit/)
