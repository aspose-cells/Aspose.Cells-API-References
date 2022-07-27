---
title: FormatCondition
second_title: Aspose.Cells لمرجع .NET API
description: يمثل شرط التنسيق الشرطي.
type: docs
weight: 3560
url: /ar/net/aspose.cells/formatcondition/
---
## FormatCondition class

يمثل شرط التنسيق الشرطي.

```csharp
public class FormatCondition
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | احصل على مثيل التنسيق الشرطي "AboveAverage" . تسلط قاعدة المثيل الافتراضية الضوء على الخلايا التي تكون أعلى من المتوسط لجميع القيم في النطاق. صالحة فقط للنوع = AboveAverage . |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | احصل على مثيل "ColorScale" الخاص بالتنسيق الشرطي . المثيل الافتراضي هو "أخضر-أصفر-أحمر" 3ColorScale . صالح فقط للنوع = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | احصل على مثيل "DataBar" الخاص بالتنسيق الشرطي. اللون الافتراضي للمثيل هو الأزرق . صالح فقط للنوع هو DataBar . |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | الحصول على القيمة أو التعبير المرتبط بالتنسيق الشرطي وتعيينهما. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | الحصول على القيمة أو التعبير المرتبط بالتنسيق الشرطي وتعيينهما. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | احصل على مثيل "IconSet" للتنسيق الشرطي . IconSetType للمثيل الافتراضي هو TrafficLights31. صالح فقط للنوع = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | الحصول على نوع عامل التنسيق الشرطي وتعيينه. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وتقديمه. القيم الرقمية الأقل أولوية أعلى من القيم الرقمية الأعلى ، حيث "1" هي الأولوية القصوى . |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | صحيح ، لا يمكن تطبيق أي قواعد ذات أولوية أقل على هذه القاعدة ، عندما يتم تقييم هذه القاعدة إلى "صحيح". تنطبق فقط على Excel 2007 ؛ |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | الحصول على أو ضبط نمط نطاقات الخلايا المنسقة الشرطية. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | قيمة النص في قاعدة التنسيق الشرطي "نص يحتوي على". صالح فقط للنوع = يحتوي على نص ، وليس يحتوي على نص ، ويبدأ مع وينتهي . القيمة الافتراضية هي خالية. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | الفترة الزمنية القابلة للتطبيق في قاعدة التنسيق الشرطي "تاريخ حدوث ...". صالح فقط للنوع = timePeriod. القيمة الافتراضية هي TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | احصل على مثيل "Top10" الخاص بالتنسيق الشرطي . تسلط قاعدة المثيل الافتراضية الضوء على الخلايا التي تقع قيمها في أعلى 10 فئة . صالحة فقط للنوع هو Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | يحصل على نوع التنسيق الشرطي ويعينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | الحصول على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | الحصول على صيغة التنسيق الشرطي للخلية. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | الحصول على قيمة أو تعبير التنسيق الشرطي للخلية. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | الحصول على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | الحصول على صيغة التنسيق الشرطي للخلية. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | الحصول على قيمة أو تعبير التنسيق الشرطي للخلية. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |

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

[VB.NET]

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
