---
title: HyperlinkLoadMode
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Specifies how hyperlinks are handled when loading HTML.
type: docs
url: /javascript-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode enumeration
Specifies how hyperlinks are handled when loading HTML.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Only the first hyperlink in a cell is loaded, subsequent ones are ignored. |
| AllowMultiple | `1` | All hyperlinks in a cell are added to [Worksheet.Hyperlinks](../worksheet.hyperlinks/). Note that MS Excel itself supports only one hyperlink per cell, so this option may produce files that Excel cannot fully render. |

