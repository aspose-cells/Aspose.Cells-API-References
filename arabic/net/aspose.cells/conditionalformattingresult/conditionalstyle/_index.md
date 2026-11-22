---
title: "ConditionalFormattingResult.ConditionalStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingResult. تحصل على نمط النتيجة الشرطية"
type: docs
url: /ar/net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

يحصل على نمط النتيجة الشرطية.

```csharp
public Style ConditionalStyle { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            
            // أنشئ شرطًا واضبط النمط
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            fc.Style = style;

            // احصل على الخلية ذات التنسيق الشرطي
            Cell cell = worksheet.Cells["A3"];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            
            // أخرج اللون لعرض الخاصية
            Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


