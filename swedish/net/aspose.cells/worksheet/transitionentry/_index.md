---
title: "Worksheet.TransitionEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om alternativet för Lotus‑kompatibilitet för Transition Formula Entry är aktiverat"
type: docs
url: /sv/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Anger om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat.

```csharp
public bool TransitionEntry { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in TransitionEntry‑egenskapen
            worksheet.TransitionEntry = true;
            
            // Visa TransitionEntry‑värdet
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visa det inlästa TransitionEntry‑värdet
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


