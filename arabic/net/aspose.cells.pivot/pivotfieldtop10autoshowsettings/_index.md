---
title: "فئة PivotFieldTop10AutoShowSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Pivot.PivotFieldTop10AutoShowSettings. يمثل إعدادات العرض التلقائي لأفضل 10 لحقل محوري."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class

يمثل إعدادات العرض التلقائي لأفضل 10 لحقل محوري.

```csharp
public class PivotFieldTop10AutoShowSettings
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/autoshowcount/) { get; set; } | يمثل عدد العناصر العليا أو السفلى التي يتم عرضها تلقائيًا في حقل PivotTable المحدد. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/isautoshow/) { get; set; } | يشير إلى ما إذا كان تم تطبيق مرشح \"Top 10 AutoShow\" على هذا الحقل. |
| [IsTop](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/istop/) { get; set; } | يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا بترتيب تصاعدي. |
| [RankBy](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/rankby/) { get; set; } | يحدد فهرس حقل البيانات لتصنيف AutoShow. يمثل فهرس الحقل المعروض تلقائيًا. -1 يعني حقل PivotField نفسه. يجب أن يكون فهرس حقول البيانات. |

### ملاحظات

في ملفات xls: تنفيذ مرشحات أعلى 10 في Xls عبر Top 10 AutoShow. في ملفات ooxml: يدعم تنسيق ملف ooxml الأساسي خاصية Top10 AutoShow، لكن واجهة المستخدم في Excel 2007 وما بعده توفر الوصول فقط عبر مرشح Top10. إذا لم تكن توافقية XLS مطلوبة، يُنصح باستخدام مرشح Top10 بدلاً من ذلك.

### أمثلة

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

PivotTable pivot = pivots.Add("=Sheet1!A1:C9", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
           
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
           
 //تغيير سمات PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//عرض أعلى عنصرين حسب تسمية حقل الصف.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.Top10AutoShowSettings;
Console.WriteLine(sortSetting.IsAutoShow);

 pivot.CalculateData();

book.Save("out.xlsx");

[Visual Basic]

Dim book As New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells
cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables

Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C9", "A12")
 
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
pivot.AddFieldToArea(PivotFieldType.Column, "year")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Show top 2 items by row field label.
rowField.Top10AutoShow(True, True, 2, -1)

Dim sortSetting As PivotFieldTop10AutoShowSettings = rowField.Top10AutoShowSettings
Console.WriteLine(sortSetting.IsAutoShow)

pivot.CalculateData()

book.Save("out.xlsx")
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


