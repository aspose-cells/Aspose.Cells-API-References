---
title: "الفئة ConditionalFormattingValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.ConditionalFormattingValue. تصف قيم نقاط الاستيفاء في شريط البيانات أو مجموعة الأيقونات ذات المقياس المتدرج"
type: docs
url: /ar/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

يصف قيم نقاط الاستيفاء في مقياس متدرج أو شريط بيانات أو مجموعة أيقونات.

```csharp
public class ConditionalFormattingValue
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | احصل على أو اضبط علامة أكبر من أو يساوي. استخدمها فقط لمجموعات الأيقونات، تحدد ما إذا كانت قيمة العتبة تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى أن 'greater than' تُستخدم بدلاً من 'greater than or equal to'. القيمة الافتراضية هي true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | احصل على أو اضبط نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيؤدي تلقائيًا إلى تعيين \"Value\" إلى null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | احصل على أو اضبط قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالتزامن مع Type. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // ضبط الخصائص لـ ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // ضبط القيمة الدنيا
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // ضبط القيمة المتوسطة
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // ضبط القيمة القصوى
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // احفظ المصنف
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


