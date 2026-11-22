---
title: "الفئة FormatCondition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FormatCondition. تمثل شرط تنسيق شرطي"
type: docs
url: /ar/net/aspose.cells/formatcondition/
---
## FormatCondition class

يمثل شرط تنسيق شرطي.

```csharp
public class FormatCondition
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | احصل على نسخة "AboveAverage" من تنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تكون فوق المتوسط لجميع القيم في النطاق. صالحة فقط للنوع = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | احصل على نسخة "ColorScale" من تنسيق الشرطي. النسخة الافتراضية هي "green-yellow-red" 3ColorScale. صالحة فقط للنوع = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | احصل على نسخة "DataBar" من تنسيق الشرطي. لون النسخة الافتراضية هو الأزرق. صالحة فقط للنوع هو DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | احصل على نسخة "IconSet" من تنسيق الشرطي. نوع IconSetType للنسخة الافتراضية هو TrafficLights31. صالحة فقط للنوع = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | يحصل ويضبط نوع عامل تنسيق الشرطي. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من القيم الرقمية الأعلى، حيث أن '1' هي أعلى أولوية. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | صحيح، لا يمكن تطبيق أي قواعد ذات أولوية أقل فوق هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛ |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | القيمة النصية في قاعدة تنسيق شرطي "text contains". صالحة فقط للنوع = containsText, notContainsText, beginsWith و endsWith. القيمة الافتراضية هي null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | الفترة الزمنية القابلة للتطبيق في قاعدة تنسيق شرطي "date occurrin". صالحة فقط للنوع هو timePeriod. القيمة الافتراضية هي TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | احصل على نسخة "Top10" من تنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تقع قيمها في أعلى 10 نطاقات. صالحة فقط للنوع هو Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | يحصل ويضبط ما إذا كان نوع التنسيق الشرطي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | يحصل على الصيغة الخاصة بالتنسيق الشرطي للخلية. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | يحصل على القيمة أو التعبير الخاص بالتنسيق الشرطي للخلية. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | يحصل على الصيغة الخاصة بالتنسيق الشرطي للخلية. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | يحصل على القيمة أو التعبير الخاص بالتنسيق الشرطي للخلية. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // إنشاء مصنف جديد.
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى.
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يحدد نطاق التنسيق الشرطي.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // يضيف شرطاً.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // ضبط الخصائص
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // عرض خصائص أخرى
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // حفظ ملف Excel
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


