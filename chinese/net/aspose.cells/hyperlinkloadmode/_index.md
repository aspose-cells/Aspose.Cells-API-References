---
title: "枚举 HyperlinkLoadMode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.HyperlinkLoadMode 枚举。指定在加载 HTML 时如何处理超链接"
type: docs
url: /zh/net/aspose.cells/hyperlinkloadmode/
---
## HyperlinkLoadMode enumeration

指定在加载 HTML 时如何处理超链接。

```csharp
public enum HyperlinkLoadMode
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Normal | `0` | 仅加载单元格中的第一个超链接，后续的将被忽略。 |
| AllowMultiple | `1` | 单元格中的所有超链接都会添加到 [`Hyperlinks`](../worksheet/hyperlinks/)。请注意，MS Excel 本身每个单元格仅支持一个超链接，因此此选项可能生成 Excel 无法完全呈现的文件。 |

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


