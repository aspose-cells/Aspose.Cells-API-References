---
title: Enum HyperlinkLoadMode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HyperlinkLoadMode enum. Specifies how hyperlinks are handled when loading HTML
type: docs
url: /net/aspose.cells/hyperlinkloadmode/
---
## HyperlinkLoadMode enumeration

Specifies how hyperlinks are handled when loading HTML.

```csharp
public enum HyperlinkLoadMode
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Only the first hyperlink in a cell is loaded, subsequent ones are ignored. |
| AllowMultiple | `1` | All hyperlinks in a cell are added to [`Hyperlinks`](../worksheet/hyperlinks/). Note that MS Excel itself supports only one hyperlink per cell, so this option may produce files that Excel cannot fully render. |

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


