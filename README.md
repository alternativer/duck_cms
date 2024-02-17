![137](https://github.com/alternativer/duck_cms/assets/7103414/ffdddc1b-208e-425b-8c82-7babe4c02d5e)
# DuckCMS

> Performance without compromising productivity.

DuckCMS is a content management system (CMS) built with Phoenix LiveView. It brings the rendering speed benefits of Phoenix to even the most content-heavy pages with faster render times to boost SEO performance.

## Status

Pre-release version. You can expect incomplete features and breaking changes before a stable v0.1.0 is released.

Main components:
- Core - A functional website can be built and deployed by inserting components in database and running a server
- Admin - LiveView UI to manage layouts, pages, and all other resources. 
- Page Builder - An easy to use, drag & drop UI for building pages, targeted to non-technical users. Not released yet, in the initial stages of development.

## Local Development

The file `dev.exs` is a self-contained Phoenix application running DuckCMS with sample data and code reloading enabled. Follow these steps to get a site up and running:

1. Install dependencies, build assets, and run database setup:

```sh
mix setup
```

If deps compilation fails, make sure your environment has the compilers installed.
On Ubuntu look for the `build_essential` package, on macOS install utilities with `xcode-select --install`

2. Execute the dev script:

```sh
iex --sname core -S mix dev
```

Note that running a named node isn't required unless you're running DuckCMS LiveAdmin too.

Finally, visit any of the routes defined in `dev.exs` as http://localhost:4001/dev/home
or request resources from the API as http://localhost:4001/api/pages
