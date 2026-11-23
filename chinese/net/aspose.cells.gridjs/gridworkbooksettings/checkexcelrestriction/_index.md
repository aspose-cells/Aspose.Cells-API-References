---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridWorkbookSettings 属性。是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值，例如通过 Cell.PutValuestring 时，如果此属性为 true，您将收到异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，后续不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。默认值为 false"
type: docs
url: /zh/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值，例如通过 Cell.PutValue(string) 时，如果此属性为 true，您将收到异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，后续不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。默认值为 false。

```csharp
public bool CheckExcelRestriction { get; set; }
```

### 另请参见

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


