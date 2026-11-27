---
title: "Cells.GetViewRowHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar höjden på en specificerad rad i tum."
type: docs
url: /sv/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Hämtar höjden på en specificerad rad i enhet tum.

```csharp
public double GetViewRowHeightInch(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |

### Returvärde

Radhöjd

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange anpassad radhöjd för rad 2 i tum
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Anropa GetViewRowHeightInch med radindexparameter
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Visa resultatet och verifiera att höjden matchar det angivna värdet
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Visa effekten genom att lägga till exempelinnehåll
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Spara den modifierade arbetsboken
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


