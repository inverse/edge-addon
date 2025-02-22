# Edge Addon Action

This action will publish your addon to the Edge Web Store.

Built using the [Edge Addons API](https://github.com/inverse/python-edge-addons-api) package.

## Usage

```yaml
steps:
  - uses: inverse/edge-addon@v1.0.1
    with:
      product_id: ${{ secrets.EDGE_PRODUCT_ID }}
      client_id: ${{ secrets.EDGE_CLIENT_ID }}
      api_key: ${{ secrets.EDGE_CLIENT_SECRET }}
      zip: build/edge-addon.zip
      notes: New version upload # Could be derived from release notes
```

## Credentials

Follow the official [Using Addons API](https://learn.microsoft.com/en-us/microsoft-edge/extensions-chromium/publish/api/using-addons-api) documentation.

## License

MIT
