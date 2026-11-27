---
title: "Cells.SetRowHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Ställer in radhöjd i tum."
type: docs
url: /sv/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Ställer in radens höjd i enhet tum.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| tum | Double | Antal tum. Det bör vara mellan 0 och 409,5/72. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in standardstil
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Ställ in radhöjder i tum
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Spara arbetsboken
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


