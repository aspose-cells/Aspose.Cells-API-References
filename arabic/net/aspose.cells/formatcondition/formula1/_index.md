---
title: "FormatCondition.Formula1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. يحصل أو يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي.

```csharp
public string Formula1 { get; set; }
```

### ملاحظات

يرجى إضافة جميع المناطق قبل ضبط الصيغة. لضبط الصيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فستُعامل كصيغة. وإلا ستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: \"=\\\"=...\\\"\".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["E1"].PutValue(50);
            
            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // حدد النطاق ونوع الشرط
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // الوصول إلى خاصية Formula1 وعرضها
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


