---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Hämtar och anger antalet kolumner med text i den avgränsande rektangeln"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Hämtar och anger antalet kolumner med text i den avgränsande rektangeln.

```csharp
public int NumberOfColumns { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Ange text för formen
            shape.Text = "This is sample text\nin multiple columns";
            
            // Kom åt textjustering och ställ in antalet kolumner
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera egenskapen
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


