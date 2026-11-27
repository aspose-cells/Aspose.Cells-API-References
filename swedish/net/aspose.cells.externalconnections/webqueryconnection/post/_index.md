---
title: "WebQueryConnection.Post"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Returnerar eller anger strängen som används med POST‑metoden för att skicka data till en webbserver för att returnera data från en webbförfrågan"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Returnerar eller anger strängen som används med POST-metoden för att skicka data till en webbserver för att returnera data från en webbfråga.

```csharp
public string Post { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en webbförfrågningsanslutning genom att komma åt en befintlig eller skapa genom korrekt initiering
                // Eftersom vi inte kan instansiera WebQueryConnection direkt, använder vi den första anslutningen om den finns
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Om inga anslutningar finns, kommer vi att demonstrera med en mock-anslutning
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Ange initialt Post-värde
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Ändra Post-värdet
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Rensa Post-värdet
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Spara arbetsboken
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


