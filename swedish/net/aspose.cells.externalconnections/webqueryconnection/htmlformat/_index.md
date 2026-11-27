---
title: "WebQueryConnection.HtmlFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Hur man hanterar formatering från HTML‑källan när webbförfrågningsdata förs in i kalkylbladet. Relevant när sourceData är True"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Hur formatering från HTML-källan ska hanteras när webbfrågedata förs in i kalkylbladet. Relevant när sourceData är True.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till den första befintliga webbfrågeanslutningen (om någon)
            // Eller skapa en ny genom att läsa in en fil med webbanslutningar
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Visa initialt HtmlFormat‑värde
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Ställ in HtmlFormat till Rtf (demonstrerar skrivoperation)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Ställ in HtmlFormat till None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Spara arbetsboken med webbförfrågningsanslutningen
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### Se även

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


