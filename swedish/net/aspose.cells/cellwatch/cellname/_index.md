---
title: "CellWatch.CellName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellWatch-egenskap. Hämtar och anger namnet på cellen"
type: docs
url: /sv/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Hämtar och anger namnet på cellen.

```csharp
public string CellName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några cellövervakningar
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Visa cellnamn för alla övervakningar
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Lägg till en ny övervakning och visa dess namn
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Spara arbetsboken
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


