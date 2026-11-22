---
title: "فئة PivotCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridWeb.Data.PivotCache. تمثل الذاكرة المؤقتة لتقرير PivotTable. كائن PivotCache هو عضو في مجموعة PivotCaches"
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

تمثل الذاكرة المؤقتة لتقرير PivotTable. كائن PivotCache هو عضو في مجموعة [`PivotCaches`](../pivotcaches/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | يرجع مصدر البيانات لـ System.Data.DataTable لتقرير PivotTable. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | يرجع مصدر البيانات لـ System.Data.DataView لتقرير PivotTable. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | يرجع الفهرس لهذا الكائن في Parent |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | يرجع اسم PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | يرجع الكائن الأب للعنصر المحدد (حاوية PivotCache). للقراءة فقط. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | يرجع نطاق مصدر البيانات باستخدام SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | يرجع مصدر البيانات لـ WebWorksheet لتقرير PivotTable. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | يمثل نوع بيانات المصدر |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | ينشئ تقرير PivotTable إلى ورقة جديدة. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | ينشئ تقرير PivotTable إلى ورقة جديدة. اسم كائن pivotTable |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | ينشئ تقرير PivotTable إلى targetSheet. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | ينشئ تقرير PivotTable إلى targetSheet. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | يحدد ما إذا كانت مثيلتا Object متساويتين. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | يعمل كدالة تجزئة لنوع معين، مناسبة للاستخدام في خوارزميات التجزئة وهياكل البيانات مثل جدول التجزئة. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | يعيد تعيين بيانات المصدر |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | يعيد تعيين بيانات المصدر |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | يعيد تعيين بيانات المصدر |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | يرجع سلسلة تمثل الكائن الحالي |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridPivotTable بدلاً منها. سيتم إزالة هذه الفئة بعد 6 أشهر منذ أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

يستخدم طريقة PivotCache لإرجاع كائن PivotCache لتقرير PivotTable (كل تقرير يحتوي على مخزن واحد فقط). بيانات المصدر لـ PivotCache تأتي من WebWorksheet و DataTable، وما إلى ذلك.

### أمثلة

```csharp

 [C#]

 //بافتراض أن ورقة العمل \"Sheet1\" تحتوي على بيانات، يتم إنشاء تقرير PivotTable بناءً عليها.
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

 //ينشئ تقرير PivotTable من DataView أو DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Or PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
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

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


