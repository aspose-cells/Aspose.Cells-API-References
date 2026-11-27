---
title: "Worksheet.IsGridlinesVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar eller anger ett värde som indikerar om rutnätslinjerna är synliga. Default är true"
type: docs
url: /sv/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Hämtar eller anger ett värde som indikerar om rutnätslinjerna är synliga. Standard är sant.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in rutnätslinjernas synlighet till true
            worksheet.IsGridlinesVisible = true;
            
            // Lägg till exempeldata för att se rutnätslinjer
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Autoanpassa kolumner för bättre synlighet
            worksheet.AutoFitColumns();
            
            // Spara arbetsboken
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


