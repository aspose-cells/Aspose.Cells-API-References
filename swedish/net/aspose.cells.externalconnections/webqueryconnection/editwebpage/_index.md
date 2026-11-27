---
title: "WebQueryConnection.EditWebPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. URL:en för den användarorienterade webbsidan som visar webbförfrågningsdata. Denna URL sparas för det fall att sourceDatatrue och url har omdirigerats för att referera till en XML‑fil. Då kan den användarorienterade sidan visas i UI och XML‑data kan hämtas i bakgrunden."
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

URL:en för den användarorienterade webbsidan som visar webbfrågedata. Denna URL sparas om sourceData=\"true\" och url har omdirigerats för att referera till en XML-fil. Då kan den användarorienterade sidan visas i UI:t, och XML-data kan hämtas i bakgrunden.

```csharp
public string EditWebPage { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första befintliga webbfrågeanslutningen (om någon)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Ställ in initialt värde för EditWebPage
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Uppdatera EditWebPage‑värdet
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Spara arbetsboken med webbförfrågningsanslutningen
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


