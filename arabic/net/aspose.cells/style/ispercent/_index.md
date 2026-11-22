---
title: "Style.IsPercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان تنسيق الرقم هو تنسيق نسبة مئوية"
type: docs
url: /ar/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

يشير إلى ما إذا كان تنسيق الرقم هو تنسيق نسبة مئوية.

```csharp
public bool IsPercent { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية A1 وتعيين قيمتها
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // احصل على نمط الخلية
            Style style = cell.GetStyle();
            
            // عرض قيمة IsPercent الحالية
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // تعيين تنسيق الرقم إلى النسبة المئوية (سيؤدي ذلك تلقائيًا إلى تعيين IsPercent إلى true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // تحقق من أن IsPercent الآن true
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // إنشاء خلية أخرى بتنسيق مختلف
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // تحقق من أن IsPercent هو false لتنسيق غير نسبي
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // احفظ المصنف
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


