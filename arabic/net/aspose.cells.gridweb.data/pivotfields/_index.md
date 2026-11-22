---
title: "الفئة PivotFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.PivotFields. تمثل مجموعة من جميع كائنات PivotField في تقرير PivotTable"
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

تمثل مجموعة من جميع كائنات [`PivotField`](../pivotfield/) في تقرير PivotTable.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | يحصل على عدد العناصر الموجودة في مثيل PivotFields |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الوصول إلى PivotFields متزامنًا (آمن للخيوط). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | يحصل على PivotField حسب الفهرس. (2 مؤشرات) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | يحصل على الكائن الأب للكائن المحدد. للقراءة فقط. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | يحصل على كائن يمكن استخدامه لمزامنة الوصول إلى PivotFields. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | ينسخ كامل PivotField إلى مصفوفة أحادية البعد متوافقة، بدءًا من الفهرس المحدد للمصفوفة الهدف. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | يرجع IEnumerator لـ PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | يحصل على فهرس PivotField المحدد. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridPivotFieldCollection بدلاً منها. سيتم إزالة هذه الفئة بعد 6 أشهر من أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

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


