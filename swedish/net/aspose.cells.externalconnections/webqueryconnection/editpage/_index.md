---
title: "WebQueryConnection.EditPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. URL:en för den användarorienterade webbsidan som visar webbförfrågningsdata. Denna URL sparas för det fall att sourceDatatrue och url har omdirigerats för att referera till en XML‑fil. Då kan den användarorienterade sidan visas i UI och XML‑data kan hämtas i bakgrunden."
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

URL:en för den användarorienterade webbsidan som visar webbfrågedata. Denna URL sparas om sourceData=\"true\" och url har omdirigerats för att referera till en XML-fil. Då kan den användarorienterade sidan visas i UI:t, och XML-data kan hämtas i bakgrunden.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen WebQueryConnection.EditWebPage. Denna egenskap kommer att tas bort 12 månader senare sedan oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Kom åt den första befintliga webbförfrågningsanslutningen om den finns
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt EditPage-värde
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Ange EditPage till en ny URL (eftersom den är läs-skriv)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


