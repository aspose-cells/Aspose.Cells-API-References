---
title: "类 PivotCache"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.PivotCache 类。表示 PivotTable 报表的内存缓存。PivotCache 对象是 PivotCaches 集合的成员。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

表示 PivotTable 报表的内存缓存。PivotCache 对象是 [`PivotCaches`](../pivotcaches/) 集合的成员。

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | 返回用于 PivotTable 报表的 System.Data.DataTable 数据源。 |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | 返回用于 PivotTable 报表的 System.Data.DataView 数据源。 |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | 返回此对象在 Parent 中的索引 |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | 返回 PivotCache.Re 的名称 |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | 返回指定对象（PivotCache 的容器）的父对象。只读。 |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | 返回使用 SourceSheet 的数据源范围。 |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | 返回用于 PivotTable 报表的 WebWorksheet 数据源。 |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | 表示源数据的类型 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | 在新工作表中创建 PivotTable 报表。 |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | 在新工作表中创建 PivotTable 报表。pivotTable 对象的名称 |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | 在 targetSheet 中创建 PivotTable 报表。 |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | 在 targetSheet 中创建 PivotTable 报表。 |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | 确定两个 Object 实例是否相等。 |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | 作为特定类型的哈希函数，适用于哈希算法和哈希表等数据结构。 |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | 重置源数据 |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | 重置源数据 |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | 重置源数据 |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | 返回表示当前 Object 的字符串 |

### 备注

注意：此类已过时。请改用 GridPivotTable。该类将在自 2014 年 8 月起 6 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

使用 PivotCache 方法返回 PivotTable 报表的 PivotCache 对象（每个报表仅有一个缓存）。PivotCache 的源数据来自 WebWorksheet、DataTable 等。

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


