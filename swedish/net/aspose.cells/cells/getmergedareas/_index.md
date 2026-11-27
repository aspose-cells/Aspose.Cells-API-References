---
title: "Cells.GetMergedAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar alla sammanslagna celler"
type: docs
url: /sv/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Hämtar alla sammanslagna celler.

```csharp
public CellArea[] GetMergedAreas()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa några sammanslagna celler
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Hämta alla sammanslagna områden
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Visa information om sammanslagna områden
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


