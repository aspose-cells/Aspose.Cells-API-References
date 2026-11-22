---
title: "CellsHelper.DPI"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل على DPI للجهاز"
type: docs
url: /ar/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

يحصل على DPI للجهاز.

```csharp
public static double DPI { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // اضبط واعرض DPI الحالي
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // غيّر إعداد DPI
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // أنشئ دفتر عمل جديد واحفظه بإعدادات DPI مختلفة
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف شكلًا تجريبيًا لتوضيح تأثير DPI
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // احفظ باستخدام إعداد DPI الحالي
            workbook.Save("output_with_dpi_300.xlsx");

            // غيّر DPI واحفظ مرة أخرى
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


