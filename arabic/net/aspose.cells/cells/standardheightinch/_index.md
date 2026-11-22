---
title: "Cells.StandardHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل أو تعين ارتفاع الصف الافتراضي في هذه ورقة العمل بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

يحصل أو يعيّن ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البوصة.

```csharp
public double StandardHeightInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على الارتفاع القياسي بالبوصة
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // عيّن ارتفاعًا قياسيًا جديدًا (1 بوصة)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


