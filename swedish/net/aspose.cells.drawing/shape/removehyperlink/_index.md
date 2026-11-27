---
title: "Shape.RemoveHyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Tar bort hyperlänken för figuren"
type: docs
url: /sv/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Tar bort hyperlänken för formen.

```csharp
public void RemoveHyperlink()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en figur och ange hyperlänk
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Ta bort hyperlänken
            shape.RemoveHyperlink();

            // Verifiera att hyperlänken har tagits bort
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Spara arbetsboken
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


