# vanity

Vanity is for setting the [custom import
path](https://pkg.go.dev/cmd/go#hdr-Remote_import_paths) (`go.inflx.dev`) for
our Go packages.

For example,

```go
import "go.inflx.dev/bronze"
```

## Onboarding a New Pacakge

To onboard a new package, create a corresponding HTML file under the root
directory with the required `<meta>` tags containing the repository information.
See [`bronze.html`](bronze.html) as an example.

```html
<meta name="go-import" content="import-prefix vcs repo-root">
```