---
title: "اسم الفئة"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Name. تمثل اسمًا معرفًا لنطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/name/
---
## Name class

يمثل اسمًا معرفًا لنطاق من الخلايا.

```csharp
public class Name
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | يحصل على تعليق الاسم ويضبطه. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | يحصل على النص الكامل لاسم الكائن مع إعداد النطاق. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | يشير إلى ما إذا كان هذا الاسم مُشارًا إليه من قبل صيغ أخرى. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | يشير إلى ما إذا كان الاسم مرئيًا. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | يحصل على أو يضبط إشارة R1C1 للـ `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | يعيد أو يضبط الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | يشير إلى أن هذا الاسم ينتمي إلى مصنف Workbook أو ورقة Worksheet. 0 = اسم عالمي، وإلا فالمؤشر إلى الورقة (مؤشر يبدأ من 1). |
| [Text](../../aspose.cells/name/text/) { get; set; } | يحصل على نص اسم الكائن. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. إذا لم تكن إشارة هذا الاسم مطلقة، قد يكون النطاق مختلفًا لخلايا مختلفة. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | يحصل على جميع النطاقات التي يُشير إليها هذا الاسم. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | يحصل على جميع النطاقات التي يُشير إليها هذا الاسم. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | يحصل على جميع الإشارات التي يُشير إليها هذا الاسم. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | احصل على إشارة هذا الاسم. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | احصل على إشارة هذا الاسم بناءً على الخلية المحددة. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | اضبط إشارة هذا الاسم. |
| override [ToString](../../aspose.cells/name/tostring/)() | يعيد سلسلة تمثل كائن النطاق الحالي. |

### أمثلة

```csharp

[C#]

//إنشاء كائن Workbook
Workbook workbook = new Workbook();
//الوصول إلى ورقة العمل الأولى في ملف Excel
Worksheet worksheet = workbook.Worksheets[0];
//إنشاء نطاق مسمى
Range range = worksheet.Cells.CreateRange("B4", "G14");
//تعيين اسم النطاق المسمى
range.Name = "TestRange";
//حفظ ملف Excel المعدل بالتنسيق الافتراضي (وهو Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


