---
title: "WebQueryConnection.IsParsePre"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Flagga som indikerar om data som finns inom HTML PRE‑taggar på webbsidan parsas till kolumner när du importerar sidan till en frågetabell"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Flagga som anger om data som finns inom HTML PRE-taggar på webbsidan ska parsas till kolumner när du importerar sidan till en frågetabell.

```csharp
public bool IsParsePre { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en ny webbförfrågningsanslutning med den befintliga anslutningen från arbetsboken
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Visa initialt IsParsePre‑värde (standard)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Ställ in IsParsePre till true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Ställ in IsParsePre tillbaka till false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Spara arbetsboken
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


