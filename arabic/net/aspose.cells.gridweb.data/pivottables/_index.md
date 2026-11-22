---
title: "الفئة PivotTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridWeb.Data.PivotTables class. يمثل مجموعة من جميع كائنات PivotTable"
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

يمثل مجموعة من جميع كائنات [`PivotTable`](../pivottable/)

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | يحصل على عدد العناصر الموجودة في مثيل PivotTables |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الوصول إلى PivotTables متزامنًا (آمن للخيوط). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | يحصل على كائن PivotTable حسب الفهرس. (مؤشرين) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | يحصل على الكائن الأب للكائن المحدد. للقراءة فقط. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | يحصل على كائن يمكن استخدامه لمزامنة الوصول إلى PivotTables. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | يضيف كائن PivotTable من PivotCache المحدد إلى ورقة عمل جديدة |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | يضيف كائن PivotTable من PivotCache المحدد إلى ورقة عمل جديدة |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | يضيف كائن PivotTable من PivotCache المحدد إلى ورقة العمل المحددة |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | يضيف كائن PivotTable من PivotCache المحدد إلى ورقة العمل المحددة |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | يزيل جميع كائنات PivotTable وجميع كائنات PivotCache في التحكم. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | يرجع true إذا كان هناك اسم pivottable tableName موجود. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | ينسخ جدول PivotTable بالكامل إلى مصفوفة أحادية البعد متوافقة، بدءًا من الفهرس المحدد للمصفوفة الهدف. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | يعيد IEnumerator لجداول PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | يعيد ربط مصدر البيانات بتقرير PivotTable. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | يعيد ربط مصدر البيانات بجميع تقارير PivotTable. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | يزيل كائن PivotTable المحدد من PivotTables و PivotCache المرتبط إذا لم يستخدمه PivotTable آخر. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | يزيل كائن PivotTable المحدد من PivotTables و PivotCache المرتبط إذا لم يستخدمه PivotTable آخر. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridPivotTableCollection بدلاً منها. ستتم إزالة هذه الفئة بعد 6 أشهر من أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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


