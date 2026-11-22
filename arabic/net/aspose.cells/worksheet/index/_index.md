---
title: "Worksheet.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على فهرس الورقة في مجموعة الأوراق"
type: docs
url: /ar/net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

يحصل على فهرس الورقة في مجموعة أوراق العمل.

```csharp
public int Index { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ثلاث أوراق عمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // الوصول إلى أوراق العمل حسب الفهرس وعرض خاصية Index
            Console.WriteLine("Worksheet Index Demonstration:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
            }

            // إضافة بعض التنسيقات الشرطية لعرض استخدام الفهرس
            Worksheet firstSheet = workbook.Worksheets[0];
            int formatIndex = firstSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // عرض معلومات فهرس التنسيق الشرطي
            Console.WriteLine("\nConditional Formatting Indexes:");
            Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
            Console.WriteLine($"Formatting Collection Index: {formatIndex}");
            Console.WriteLine($"First Condition Index: 0");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


