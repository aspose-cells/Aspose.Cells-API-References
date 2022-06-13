---
title: CheckExcelRestriction
second_title: Aspose.Cells for .NET API 参考
description: 用户修改单元格相关对象时是否检查excel文件的限制 例如excel不允许输入超过32K的字符串值 当你输入一个超过 32K 的值时比如通过 Cell.PutValuestring如果这个属性为真你会得到一个 Exception 如果此属性为 false我们将接受您输入的字符串值作为单元格的值以便稍后 您可以为其他文件格式例如 CSV输出完整的字符串值 但是如果您设置了这种对 excel 文件格式无效的值则 以后不应将工作簿保存为 excel 文件格式否则生成的excel文件可能会出现意外错误
type: docs
weight: 70
url: /zh/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

用户修改单元格相关对象时是否检查excel文件的限制。 例如，excel不允许输入超过32K的字符串值。 当你输入一个超过 32K 的值时，比如通过 Cell.PutValue(string)，如果这个属性为真，你会得到一个 Exception。 如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后 您可以为其他文件格式（例如 CSV）输出完整的字符串值。 但是，如果您设置了这种对 excel 文件格式无效的值，则 以后不应将工作簿保存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。

```csharp
public bool CheckExcelRestriction { get; set; }
```

### 也可以看看

* class [WorkbookSettings](../../workbooksettings)
* 命名空间 [Aspose.Cells](../../workbooksettings)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->