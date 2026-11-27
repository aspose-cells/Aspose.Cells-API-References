---
title: "WebQueryConnection.IsConsecutive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. Flagga som indikerar om på varandra följande avgränsare ska behandlas som en enda avgränsare"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Flagga som anger om på varandra följande avgränsare ska behandlas som en enda avgränsare.

```csharp
public bool IsConsecutive { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en webbförfrågningsanslutning genom att komma åt den första anslutningen
            // (förutsatt att det finns minst en anslutning tillgänglig)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Visa initialt IsConsecutive‑värde (standard)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Ställ in IsConsecutive till true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Ställ in IsConsecutive tillbaka till false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Spara arbetsboken med webbförfrågningsanslutningen
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


