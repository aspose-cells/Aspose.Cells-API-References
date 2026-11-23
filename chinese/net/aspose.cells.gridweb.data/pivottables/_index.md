---
title: "类 PivotTables"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.PivotTables 类。表示所有 PivotTable 对象的集合"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

表示所有 [`PivotTable`](../pivottable/) 对象的集合

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | 获取 PivotTables 实例中包含的元素数量 |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | 获取一个值，指示对 PivotTables 的访问是否已同步（线程安全）。 |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | 通过索引获取 PivotTable 对象。（两个索引器） |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | 获取指定对象的父对象。只读。 |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | 获取可用于同步对 PivotTables 访问的对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | 将指定 PivotCache 中的 PivotTable 对象添加到新工作表中 |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | 将指定 PivotCache 中的 PivotTable 对象添加到新工作表中 |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | 将指定 PivotCache 中的 PivotTable 对象添加到指定工作表中 |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | 将指定 PivotCache 中的 PivotTable 对象添加到指定工作表中 |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | 移除控件中所有 PivotTable 对象和所有 PivotCache 对象。 |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | 如果存在名为 tableName 的 PivotTable，则返回 true。 |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | 将整个 PivotTable 复制到兼容的一维数组中，从目标数组的指定索引开始 |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | 返回 PivotTables 的 IEnumerator。 |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | 重新绑定数据源到 PivotTable 报表。 |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | 重新绑定数据源到所有 PivotTable 报表。 |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | 如果未被其他 PivotTable 使用，则从 PivotTables 中移除指定的 PivotTable 对象并删除相关的 PivotCache。 |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | 如果未被其他 PivotTable 使用，则从 PivotTables 中移除指定的 PivotTable 对象并删除相关的 PivotCache。 |

### 备注

注意：此类已过时。请改用 GridPivotTableCollection。该类将在自 2014 年 8 月起的 6 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

### 示例

```csharp

 [C#]

 //假设工作表 "Sheet1" 中有数据，则基于它创建一个数据透视表报告。
 WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
 Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
 sourceRange.StartRow = 0;
 sourceRange.StartColumn = 0;
 sourceRange.EndRow = 10;
 sourceRange.EndColumn = 5;

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);

 PivotTable table = cache.CreatePivotTable();

 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
 table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;

 table.PivotFields[3].Function = PivotFieldFunction.Count;
 table.PivotFields[5].Function = PivotFieldFunction.Sum;

 table.DataBind();

 //从 DataView 或 DataTable 创建数据透视表报告。
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //或 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
 PivotTable table = cache.CreatePivotTable();
 table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.DataBind();


 [VB]


 'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
 Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
 Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
 sourceRange.StartRow = 0
 sourceRange.StartColumn = 0
 sourceRange.EndRow = 10
 sourceRange.EndColumn = 5

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)

 Dim table As PivotTable =  cache.CreatePivotTable()

 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
 table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField

 table.PivotFields(3).Function = PivotFieldFunction.Count
 table.PivotFields(5).Function = PivotFieldFunction.Sum

 table.DataBind()

 'Creates a PivotTable report from DataView or DataTable.

 Dim dataView As DataView ' Or Dim dataTable As DataTable
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
 'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
 Dim table As PivotTable =  cache.CreatePivotTable()
 table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.DataBind()

```

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


