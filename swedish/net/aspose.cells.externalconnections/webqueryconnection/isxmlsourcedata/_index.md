---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Flagga som indikerar att XML‑källdata ska importeras istället för själva HTML‑tabellen"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

Flagga som anger att XML-källdata ska importeras i stället för själva HTML-tabellen.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till en befintlig webbfrågeanslutning eller skapa en via korrekt initiering
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt IsXmlSourceData‑värde
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Ställ in IsXmlSourceData till true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Återställ IsXmlSourceData till false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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


