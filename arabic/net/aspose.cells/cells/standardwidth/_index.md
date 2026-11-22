---
title: "Cells.StandardWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل أو تعين عرض العمود الافتراضي في ورقة العمل بوحدة الأحرف"
type: docs
url: /ar/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف.

```csharp
public double StandardWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين العرض القياسي للأعمدة
            cells.StandardWidth = 18.25;

            // عرض العرض القياسي والعرض الفعلي للعمود الأول
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // التحقق من تطبيق العرض القياسي (تقريبًا)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


