---
title: "WebQueryConnection.IsXml"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. true om webbförfrågningskällan är XML jämfört med HTML, annars false"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true om webbfrågekällan är XML (i stället för HTML), annars false.

```csharp
public bool IsXml { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första datakopplingen (förutsatt att den är en WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt IsXml‑värde
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // Ställ in IsXml till true (eftersom den är läs‑skriv)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // Ställ in IsXml tillbaka till false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
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


