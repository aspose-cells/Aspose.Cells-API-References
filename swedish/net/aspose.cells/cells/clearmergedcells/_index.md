---
title: "Cells.ClearMergedCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Rensar alla sammanslagna områden"
type: docs
url: /sv/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Rensar alla sammanslagna områden.

```csharp
public void ClearMergedCells()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa sammanslagna celler i A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Rensa alla sammanslagna celler i kalkylbladet
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


