---
title: "FormatCondition.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. قيمة النص في قاعدة تنسيق شرطي تحتوي على نص. صالحة فقط للنوع containsText notContainsText beginsWith و endsWith. القيمة الافتراضية هي null"
type: docs
url: /ar/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

القيمة النصية في قاعدة تنسيق شرطي "text contains". صالحة فقط للنوع = containsText, notContainsText, beginsWith و endsWith. القيمة الافتراضية هي null.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // إضافة شرط نصي
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // تعيين خاصية النص (عرض نص روسي)
            formatCondition.Text = "вс";

            // تطبيق نمط التنسيق
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // تطبيق على الخلية A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // حفظ والتحقق
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


