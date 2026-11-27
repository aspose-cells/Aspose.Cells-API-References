---
title: "Worksheet.HasAutofilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om detta worksheet har autofilter"
type: docs
url: /sv/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Anger om detta kalkylblad har autofilter.

```csharp
public bool HasAutofilter { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Ställ in autofilter
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Kontrollera om worksheet har autofilter
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


