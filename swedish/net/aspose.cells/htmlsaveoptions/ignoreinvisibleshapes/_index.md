---
title: "HtmlSaveOptions.IgnoreInvisibleShapes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Ange om de osynliga formerna ska exporteras"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Anger om osynliga former ska exporteras

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIgnoreInvisibleShapesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med ett exempelarbetsblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till synliga och osynliga former
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            shape1.IsHidden = false;
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
            shape2.IsHidden = true;

            // Spara med IgnoreInvisibleShapes = true (standard)
            HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
            saveOptions1.IgnoreInvisibleShapes = true;
            workbook.Save("output_ignore_invisible.html", saveOptions1);

            // Spara med IgnoreInvisibleShapes = false
            HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
            saveOptions2.IgnoreInvisibleShapes = false;
            workbook.Save("output_include_invisible.html", saveOptions2);

            Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


