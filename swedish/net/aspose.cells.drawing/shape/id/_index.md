---
title: "Shape.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar identifieraren för denna figur"
type: docs
url: /sv/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Hämtar identifieraren för denna form.

```csharp
public int Id { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Hämta och visa figurens ID
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Ändra figurens egenskaper
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Spara arbetsboken
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


