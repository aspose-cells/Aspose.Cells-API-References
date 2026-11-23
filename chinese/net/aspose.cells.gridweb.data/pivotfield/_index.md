---
title: "类 PivotField"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.PivotField 类。表示 PivotTable 报表中的字段。PivotField 对象是 PivotFields 集合的成员。 注意：此类已过时。请改用 GridPivotField。该类将在自 2014 年 8 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

表示 PivotTable 报表中的字段。PivotField 对象是 [`PivotFields`](../pivotfields/) 集合的成员。 注意：此类已过时。请改用 GridPivotField。该类将在自 2014 年 8 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | 报告中显示的透视字段标签文本。默认显示名称。 |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | 获取指定字段的数据。 |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | 表示用于汇总 PivotTable 字段（仅数据字段）的函数。默认函数是 Count。 |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | 获取名称。 |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | 表示指定 PivotTable 报表中字段的位置。 |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | 表示字段在其方向（行、列、页）中所有字段的位置（第一、第二、第三等）。在调用 Pivottable.DataBind 后应调用获取方法。 |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | 表示用于对指定 PivotTable 字段进行排序的顺序。 |

### 示例

```csharp

 [C#]

 //获取 PivotTable[0] 的 PivotFields
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //设置 PivotFields 的位置
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //设置数据字段的函数
 field3.Function = PivotFieldFunction.Sum;

 //更改行字段的顺序
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


