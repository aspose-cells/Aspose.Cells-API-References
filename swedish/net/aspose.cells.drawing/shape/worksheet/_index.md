---
title: "Shape.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar Worksheet-objektet som innehåller denna form"
type: docs
url: /sv/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Hämtar [`Worksheet`](../../../aspose.cells/worksheet/) objektet som innehåller denna form.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Demonstrera användning av Worksheet-egenskap
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Skriv ut arbetsbladets namn för att visa att egenskapen fungerar
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


