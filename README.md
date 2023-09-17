# colors

```shell
go get gio.tools/colors
```

A collection of established color values using `color.NRGBA` (non-alpha-premultiplied).

```go
import "gio.tools/colors"

// Material colors such as...
colors.Pink200
colors.AmberA400
colors.BlueGrey500

// Apple foundation colors such as...
colors.IOSDarkBlue
colors.MacOSLightPurple
colors.WatchOSTeal

// CSS colors such as...
colors.AliceBlue
colors.DarkMagenta
colors.LimeGreen
colors.Red
```

## Why not alpha-premultiplied (`color.RGBA`)?

1. [Gio](https://gioui.org/) APIs use `color.NRGBA`, and the primary intent of this
   package is for use with Gio.
2. As mentioned in [the commit
   description](https://github.com/gioui/gio/commit/21ef492cc9dfd9161e9fc57df25684865cd1c847)
   when Gio switched, most APIs use non-premultiplied for the sake of clarity.
