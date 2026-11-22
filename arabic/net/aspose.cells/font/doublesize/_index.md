---
title: "Font.DoubleSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. الحصول على أو تعيين الحجم المزدوج للخط"
type: docs
url: /ar/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

يحصل على ويضبط الحجم المزدوج للخط.

```csharp
public double DoubleSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


