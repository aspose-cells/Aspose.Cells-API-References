---
title: "WebQueryConnection.Url"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. URL att använda för att uppdatera extern data"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL att använda för att uppdatera extern data.

```csharp
public string Url { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en webbförfrågningsanslutning genom att lägga till den i samlingen
            // Samlingen kommer sannolikt att skapa och returnera anslutningsobjektet
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Ange initial URL för webbförfrågan
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Ändra URL:en till en annan källa
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Konfigurera anslutningen för att tolka XML‑data
            connection.IsXml = true;

            // Uppdatera datakopplingen (skulle normalt hämta data från URL:en)
            // Obs: Faktisk webbåtkomst skulle kräva nätverksanslutning
            // workbook.RefreshAllConnections();

            // Spara arbetsboken med webbförfrågningsanslutningen
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


