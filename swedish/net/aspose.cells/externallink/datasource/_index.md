---
title: "ExternalLink.DataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink-egenskap. Representerar datakälla för den externa länken"
type: docs
url: /sv/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Representerar datakällan för den externa länken.

```csharp
public string DataSource { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en extern länk till en annan arbetsbok
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att kontrollera externa länkar
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Åtkomst till DataSource-egenskapen för den externa länken
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


