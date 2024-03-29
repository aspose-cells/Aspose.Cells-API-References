---
title: Hyperlink
second_title: Aspose.Cells for .NET API 参考
description: 封装表示超链接的对象
type: docs
weight: 3750
url: /zh/net/aspose.cells/hyperlink/
---
## Hyperlink class

封装表示超链接的对象。

```csharp
public class Hyperlink
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address) { get; set; } | 表示超链接的地址。 |
| [Area](../../aspose.cells/hyperlink/area) { get; } | 获取超链接的范围。 |
| [LinkType](../../aspose.cells/hyperlink/linktype) { get; } | 获取链接类型。 |
| [ScreenTip](../../aspose.cells/hyperlink/screentip) { get; set; } | 返回或设置指定超链接的屏幕提示文本。 |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay) { get; set; } | 表示要为指定超链接显示的文本。默认值为超链接的地址。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete)() | 删除此超链接 |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
//向Workbook对象添加一个新的工作表
workbook.Worksheets.Add();
//通过传入工作表的索引来获取新添加的工作表的引用
Worksheet worksheet = workbook.Worksheets[0];
//在“A1”单元格处添加指向 URL 的超链接
int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
//通过索引获取超链接。
Hyperlink hyperlink = worksheet.Hyperlinks[index];
//设置此超链接的显示文本。
hyperlink.TextToDisplay = "Aspose";
//保存Excel文件
workbook.Save("book1.xls");

[Visual Basic]

'实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'将新工作表添加到 Workbook 对象
workbook.Worksheets.Add()
'通过传入工作表的索引来获取新添加的工作表的引用
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Adding a hyperlink to a URL at "A1" cell
Dim index as Integer = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")
'通过索引获取超链接。
Dim hyperlink as Hyperlink = worksheet.Hyperlinks(index);
'设置此超链接的显示文本。
hyperlink.TextToDisplay = "Aspose";
'保存 Excel 文件
workbook.Save("book1.xls")
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
