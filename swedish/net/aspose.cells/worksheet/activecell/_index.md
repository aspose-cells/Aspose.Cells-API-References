---
title: "Worksheet.ActiveCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Hämtar eller anger den aktiva cellen i arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Hämtar eller anger den aktiva cellen i kalkylbladet.

```csharp
public string ActiveCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in aktiv cell till B2
            worksheet.ActiveCell = "B2";
            
            // Skriv ut adressen för den aktiva cellen
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera den aktiva cellen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


