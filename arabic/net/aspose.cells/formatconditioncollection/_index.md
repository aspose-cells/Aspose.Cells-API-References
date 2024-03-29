---
title: FormatConditionCollection
second_title: Aspose.Cells لمرجع .NET API
description: يمثل التنسيق الشرطي . يمكن أن تحتوي شروط التنسيق على ما يصل إلى ثلاثة تنسيقات شرطية.
type: docs
weight: 3570
url: /ar/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

يمثل التنسيق الشرطي . يمكن أن تحتوي شروط التنسيق على ما يصل إلى ثلاثة تنسيقات شرطية.

```csharp
public class FormatConditionCollection
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count) { get; } | يحصل على عدد الشروط . |
| [Item](../../aspose.cells/formatconditioncollection/item) { get; } | يحصل على شرط التنسيق بالفهرس . |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount) { get; } | الحصول على عدد النطاقات المنسقة شرطيًا. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add)(CellArea, FormatConditionType, OperatorType, string, string) | يضيف شرط تنسيق ونطاق خلية مؤثر إلى FormatConditions يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea)(CellArea) | يضيف نطاق خلايا منسق شرطيًا. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition#addcondition)(FormatConditionType) | أضف شرط تنسيق . |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition#addcondition_1)(FormatConditionType, OperatorType, string, string) | يضيف شرط تنسيق . |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea)(int) | الحصول على نطاق الخلايا المنسق الشرطي بالفهرس. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea#removearea_1)(int) | يزيل نطاق الخلايا المنسق الشرطي بالفهرس. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea#removearea)(int, int, int, int) | إزالة التنسيق الشرطي من النطاق. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition)(int) | يزيل شرط التنسيق بالفهرس. |

### أمثلة

```csharp

[C#]

// إنشاء مصنف جديد.
Workbook workbook = new Workbook();

// احصل على ورقة العمل الأولى.
Worksheet sheet = workbook.Worksheets[0];

// يضيف تنسيقًا شرطيًا فارغًا
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// يعين نطاق التنسيق الشرطي.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
// يضيف الشرط.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
// يضيف الشرط.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
// يعين لون الخلفية.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
// حفظ ملف Excel
workbook.Save("output.xls");   

[Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
' يضيف تنسيقًا شرطيًا فارغًا
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
'يضبط نطاق التنسيق الشرطي.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
'يضيف الشرط.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
'يضيف الشرط.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
'يضبط لون الخلفية.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
'حفظ ملف Excel
workbook.Save("output.xls")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
