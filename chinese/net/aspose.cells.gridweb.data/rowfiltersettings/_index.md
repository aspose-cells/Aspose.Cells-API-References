---
title: "类 RowFilterSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings 类。RowFilter 的摘要描述"
type: docs
url: /zh/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

RowFilter 的摘要描述。

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | 过滤条件字符串。 |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | 启用自动筛选。HeaderRow 将显示下拉按钮，以便用户选择要筛选的列值。 |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | 过滤范围的结束行号。如果此值设置为 -1，则使用工作表的最后一行号。 |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | 显示过滤下拉按钮的标题行号。 |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | 过滤范围的起始行号。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | 根据自动过滤设置构建条件字符串。 |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | 清除所有过滤设置并显示所有行。 |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | 指定自定义过滤器。 |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | 使用条件字符串过滤行。 |

### 备注

注意：此类已过时。自 2014 年 8 月起 6 个月后此类将被移除。您可以使用 GridWorksheet AddAutoFilter/FilterString 进行自动过滤/自定义过滤设置。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


