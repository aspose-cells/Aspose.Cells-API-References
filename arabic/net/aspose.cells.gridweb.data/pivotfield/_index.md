---
title: "الفئة PivotField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridWeb.Data.PivotField. تمثل حقلًا في تقرير PivotTable. كائن PivotField هو عضو في مجموعة PivotFields. ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك يرجى استخدام GridPivotField. سيتم إزالة هذه الفئة بعد 6 أشهر منذ أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته."
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

تمثل حقلًا في تقرير PivotTable. كائن PivotField هو عضو في مجموعة [`PivotFields`](../pivotfields/). ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام GridPivotField. سيتم إزالة هذه الفئة بعد 6 أشهر منذ أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | نص التسمية للحقول المحورية المعروضة في التقرير. بشكل افتراضي يُظهر الاسم. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | يحصل على بيانات الحقل المحدد. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | يمثل الدالة المستخدمة لتلخيص حقل PivotTable (حقول البيانات فقط). الدالة الافتراضية هي Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | يحصل على الاسم. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | يمثل موقع الحقل في تقرير PivotTable المحدد. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | يمثل موضع الحقل (الأول، الثاني، الثالث، وهكذا) بين جميع الحقول في اتجاهه (Rows, Columns, Pages). يجب عليك استدعاء طريقة get بعد استدعاء Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | يمثل الترتيب المستخدم لفرز حقل PivotTable المحدد. |

### أمثلة

```csharp

 [C#]

 //يحصل على PivotFields من PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //يضبط موقع PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //يضبط دالة حقل البيانات
 field3.Function = PivotFieldFunction.Sum;

 //يغيّر ترتيب حقول الصف
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

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


