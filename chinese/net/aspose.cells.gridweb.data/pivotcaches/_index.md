---
title: "类 PivotCaches"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.PivotCaches 类。表示工作簿中来自 PivotTable 报表的内存缓存集合。每个内存缓存由一个 PivotCache 对象表示。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

表示工作簿中来自 PivotTable 报表的内存缓存集合。每个内存缓存由一个 [`PivotCache`](../pivotcache/) 对象表示。

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | 获取 PivotCaches 实例中包含的元素数量 |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | 获取一个值，指示对 PivotCaches 的访问是否已同步（线程安全）。 |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | 通过索引获取 PivotCache 对象。（2 个索引器） |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | 获取指定对象的父对象。只读。 |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | 获取可用于同步对 PivotCaches 访问的对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | 从 DataTable 添加 PivotCache。 |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | 从 DataView 添加 PivotCache。 |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | 使用指定名称从 DataTable 添加 PivotCahe。 |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | 使用指定名称从 DataView 添加 PivotCahe。 |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | 从工作表添加 PivotCache |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | 使用指定名称从工作表添加 PivotCache。 |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | 移除控件中所有 PivotCache 对象和所有 PivotTable 对象。 |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | 将整个 PivotCache 复制到兼容的一维数组中，从目标数组的指定索引开始。 |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | 返回 PivotCaches 的 IEnumerator。 |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | 返回集合中指定 PivotCache 的索引 |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | 使用 pivotCache 作为数据源，从 PivotCaches 中移除指定的 PivotCache 对象及相关的 PivotTable。 |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | 使用 pivotCache 作为数据源，从 PivotCaches 中移除指定的 PivotCache 对象及相关的 PivotTable。 |

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


