---
title: "PivotFields 类"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.PivotFields 类。表示 PivotTable 报表中所有 PivotField 对象的集合"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

表示 PivotTable 报表中所有 [`PivotField`](../pivotfield/) 对象的集合。

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | 获取 PivotFields 实例中包含的元素数量 |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | 获取一个值，指示对 PivotFields 的访问是否已同步（线程安全）。 |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | 通过索引获取 PivotField。（2 个索引器） |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | 获取指定对象的父对象。只读。 |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | 获取可用于同步对 PivotFields 访问的对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | 将整个 PivotField 复制到兼容的一维数组中，从目标数组的指定索引开始 |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | 返回 PivotFields 的 IEnumerator。 |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | 获取指定 PivotField 的索引。 |

### 备注

注意：此类已过时。请改用 GridPivotFieldCollection。此类将在自 2014 年 8 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


