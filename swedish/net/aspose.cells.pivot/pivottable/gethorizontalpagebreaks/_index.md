---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Hämtar horisontella sidbrytningar för denna pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Hämtar horisontella sidbrytningar för denna pivottabell.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från källfil
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Uppdatera och beräkna pivottabellsdata
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Hämta horisontella sidbrytningar
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Visa resultaten
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


