---
title: "WebQueryConnection.IsTextDates"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. Flagga som indikerar om datum ska importeras till celler i kalkylbladet som text snarare än datum"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Flagga som anger om datum ska importeras till celler i kalkylbladet som text istället för som datum.

```csharp
public bool IsTextDates { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Skapa en webbförfrågningsanslutning genom att läsa in från en befintlig fil
                // eller genom att komma åt en befintlig anslutning
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt värde för IsTextDates
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Ställ in IsTextDates till true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Ställ in IsTextDates tillbaka till false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Spara arbetsboken med webbförfrågningsanslutningen
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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


