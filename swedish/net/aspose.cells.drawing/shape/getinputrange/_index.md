---
title: "Shape.GetInputRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Hämtar intervallet som används för att fylla kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Hämtar intervallet som används för att fylla kontrollen.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

Intervallet som används för att fylla kontrollen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Lägg till en listbox-form
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Ställ in inmatningsintervallet för listboxen
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Hämta inmatningsintervallet
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


