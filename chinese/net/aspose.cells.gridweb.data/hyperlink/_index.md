---
title: "类 Hyperlink"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.Hyperlink 类。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## 属性

| 名称 | 描述 |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | 获取或设置超链接的操作类型。它可以是 ActionTpye.UrlLink 或 ActionType.CellCommand。UrlLink 类型表示超链接指向网页或邮件收件人。例如：\"http://www.aspose.com\" 或 \"mailto:admin@aspose.com\"。CellCommand 类型表示超链接将触发 CellCommand 事件，您可以处理此事件。 |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | 获取超链接的范围。 |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | 获取或设置 Cell Command 名称。 |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | 指示在用户点击此 CellCommand 超链接时是否在客户端浏览器中丢弃用户输入。可用作“undo”操作。 |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | 获取或设置超链接的图像 URL。如果设置为 null 或空字符串，超链接将仅显示其文本。 |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | 获取或设置超链接的显示文本。 |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | 获取或设置超链接的工具提示。 |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | 获取或设置 URL 字符串。 |

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


