---
title: "FormatCondition.Operator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. يحصل على ويضبط نوع مشغل التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

يحصل ويضبط نوع عامل تنسيق الشرطي.

```csharp
public OperatorType Operator { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyOperatorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // إنشاء نطاق الخلايا
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            
            // إضافة شرط
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // تعيين النمط
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;
            
            // عرض استخدام خاصية Operator
            Console.WriteLine("Operator Type: " + fc.Operator);
            if (fc.Operator == OperatorType.Between)
            {
                Console.WriteLine("Condition is set to BETWEEN values");
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


