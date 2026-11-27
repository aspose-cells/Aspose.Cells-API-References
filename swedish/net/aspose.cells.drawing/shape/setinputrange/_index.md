---
title: "Shape.SetInputRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Anger intervallet som används för att fylla kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Ställer in intervallet som används för att fylla kontrollen.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Intervallet som används för att fylla kontrollen. |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i cellerna A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Lägg till en listbox-form
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Ange inmatningsintervall för listrutan (med parametrarna String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Ange länkad cell för listrutan
            listBox.SetLinkedCell("$A$12", false, true);

            // Spara arbetsboken
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


