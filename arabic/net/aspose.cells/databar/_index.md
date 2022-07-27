---
title: DataBar
second_title: Aspose.Cells لمرجع .NET API
description: وصف قاعدة التنسيق الشرطي لشريط البيانات. تعرض قاعدة التنسيق الشرطي هذه شريط بيانات متدرج في نطاق الخلايا.
type: docs
weight: 1240
url: /ar/net/aspose.cells/databar/
---
## DataBar class

وصف قاعدة التنسيق الشرطي لشريط البيانات. تعرض قاعدة التنسيق الشرطي هذه شريط بيانات متدرج في نطاق الخلايا.

```csharp
public class DataBar
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | الحصول على لون المحور للخلايا ذات التنسيق الشرطي كأشرطة بيانات. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | الحصول على أو تعيين موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | الحصول على كائن يحدد حدود شريط البيانات . |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | الحصول على أو تعيين كيفية تعبئة شريط البيانات باللون. |
| [Color](../../aspose.cells/databar/color) { get; set; } | احصل على أو اضبط لون شريط البيانات هذا. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | الحصول على أو تحديد اتجاه عرض قاعدة البيانات. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | الحصول على كائن القيمة القصوى لشريط البيانات هذا أو تعيينه. لا يمكن تعيين قيمة خالية أو CFValueObject من النوع FormatConditionValueType. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | يمثل الحد الأقصى لطول شريط البيانات. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | الحصول على كائن القيمة الدنيا لشريط البيانات هذا أو تعيينه . لا يمكن تعيين قيمة خالية أو CFValueObject من النوع FormatConditionValueType. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | يمثل الحد الأدنى لطول شريط البيانات. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | الحصول على كائن NegativeBarFormat المرتبط بقاعدة التنسيق الشرطي لشريط البيانات. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | احصل على أو اضبط العلامة التي تشير إلى ما إذا كنت تريد إظهار قيم الخلايا التي يتم تطبيق شريط البيانات عليها. |

## طُرق

| اسم | وصف |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | عرض شريط البيانات في الخلية إلى مصفوفة بايت الصورة. |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

// يضيف تنسيقًا شرطيًا فارغًا
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

// يعين نطاق التنسيق الشرطي.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

// يضيف الشرط.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

// احصل على Databar
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

// تعيين خصائص Databar
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
// ضع قيم الخلية
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

// حفظ ملف Excel
workbook.Save("book1.xlsx");

[VB.NET]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'يضيف تنسيقًا شرطيًا فارغًا
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'يضبط نطاق التنسيق الشرطي.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'يضيف الشرط.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'احصل على Databar
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'قم بتعيين خصائص Databar
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'ضع قيم الخلية
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'حفظ ملف Excel
workbook.Save("book1.xlsx")

```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
