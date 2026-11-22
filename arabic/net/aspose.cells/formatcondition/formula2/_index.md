---
title: "FormatCondition.Formula2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. يحصل أو يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي.

```csharp
public string Formula2 { get; set; }
```

### ملاحظات

يرجى إضافة جميع المناطق قبل ضبط الصيغة. لضبط الصيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فستُعامل كصيغة. وإلا ستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: \"=\\\"=...\\\"\".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // حدد نطاق الخلية
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // أضف شرط تنسيق باستخدام Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // احصل على شرط التنسيق
            FormatCondition formatCondition = formatConditions[0];

            // إخراج الصيغ
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // احفظ المصنف
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


