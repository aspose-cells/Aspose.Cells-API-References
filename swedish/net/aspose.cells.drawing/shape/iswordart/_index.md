---
title: "Shape.IsWordArt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om denna form är en WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Anger om denna form är en word art.

```csharp
public bool IsWordArt { get; }
```

### Anmärkningar

Endast för den äldre formen i xls-filen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en WordArt-form med alla nödvändiga parametrar
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Lägg till en vanlig rektangel-form med alla nödvändiga parametrar
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Kontrollera om formerna är WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // Exempel på användning av IsWordArt-egenskapen
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


