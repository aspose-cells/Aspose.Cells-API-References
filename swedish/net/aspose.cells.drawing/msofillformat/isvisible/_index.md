---
title: "MsoFillFormat.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormat property. Anger om det finns fyllning"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Indikerar om det finns fyllning.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en exempelshape
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // Ställ in fyllningssynlighet för shape1 (synlig)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // Ställ in fyllningssynlighet för shape2 (osynlig)
            shape2.FillFormat.IsVisible = false;

            // Demonstrera användning av IsVisible-egenskapen
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // Jämför fyllningssynlighet mellan former
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // Spara arbetsboken
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


