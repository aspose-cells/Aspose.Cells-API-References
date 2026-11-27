---
title: "Shape.ControlData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar kontrollens data"
type: docs
url: /sv/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Hämtar data för kontrollen.

```csharp
public byte[] ControlData { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Åtkomst till ControlData (skrivskyddad egenskap)
            byte[] controlData = shape.ControlData;

            // Kontrollera ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


