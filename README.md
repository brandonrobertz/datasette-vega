# datasette-vega

This is Brandon's working branch. Includes the following fixes:

- allow dynamic resizing of chart [datasette-vega#32](https://github.com/simonw/datasette-vega/issues/32)
- allow hiding/showing chart [datasette-vega#36](https://github.com/simonw/datasette-vega/issues/36) [datasette-vega#17](https://github.com/simonw/datasette-vega/issues/17) [datasette-vega#PR-18](https://github.com/simonw/datasette-vega/pull/18)
- make chart show up on query page (and any page with `columns`) [datasette-vega#41](https://github.com/simonw/datasette-vega/issues/41)
- include development instructions [datasette-vega#PR-46](https://github.com/simonw/datasette-vega/pull/46)

[![PyPI](https://img.shields.io/pypi/v/datasette-vega.svg)](https://pypi.org/project/datasette-vega/)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-vega/blob/master/LICENSE)

A [Datasette](https://github.com/simonw/datasette) plugin that provides tools
for generating charts using [Vega](https://vega.github.io/).

![Datasette Vega interface](https://raw.githubusercontent.com/simonw/datasette-vega/master/datasette-vega.png)

Try out the latest master build as a live demo at https://datasette-vega-latest.datasette.io/ or try the latest release installed as a plugin at https://fivethirtyeight.datasettes.com/

To add this to your Datasette installation, install the plugin like so:

    pip install datasette-vega

The plugin will then add itself to every Datasette table view.

If you are publishing data using the `datasette publish` command, you can
include this plugin like so:

    datasette publish now mydatabase.db --install=datasette-vega

## Development

To contribute to this tool, first checkout the code. 

```bash
git clone git@github.com:simonw/datasette-vega.git
```

Then, install dependencies

```bash
npm install
```

Then, you will be able to run a hot-reloading development server.

```bash
npm run start
```
