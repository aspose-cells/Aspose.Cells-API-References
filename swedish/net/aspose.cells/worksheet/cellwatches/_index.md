---
title: "Worksheet.CellWatches"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet egenskap. Hämtar en samling av celler på detta arbetsblad som övervakas i övervakningsfönstret"
type: docs
url: /sv/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Hämtar samling av celler i detta kalkylblad som övervakas i 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i cell B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Lägg till Cell Watch för B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Visa övervakningsinformation
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Spara arbetsboken
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


