---
title: Aspose::Cells::HyperlinkLoadMode enum
linktitle: HyperlinkLoadMode
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HyperlinkLoadMode enum. Specifies how hyperlinks are handled when loading HTML in C++.'
type: docs
weight: 23300
url: /cpp/aspose.cells/hyperlinkloadmode/
---
## HyperlinkLoadMode enum


Specifies how hyperlinks are handled when loading HTML.

```cpp
enum class HyperlinkLoadMode
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | 0 | <br>Only the first hyperlink in a cell is loaded, subsequent ones are ignored. |
| AllowMultiple | 1 | <br>All hyperlinks in a cell are added to Worksheet.Hyperlinks. Note that MS Excel itself supports only one hyperlink per cell, so this option may produce files that Excel cannot fully render. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
