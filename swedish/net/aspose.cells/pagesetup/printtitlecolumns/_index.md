---
title: "PageSetup.PrintTitleColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida"
type: docs
url: /sv/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Anger de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida.

```csharp
public string PrintTitleColumns { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt sidinställning
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in kolumner för utskriftstitel så att kolumn A upprepas på varje utskriven sida
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Lägg till lite data i kolumn A för att demonstrera effekten
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Spara arbetsboken
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


