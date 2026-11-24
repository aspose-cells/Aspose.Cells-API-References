---
title: "WebQueryConnection.HtmlFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection property. Wie die Formatierung aus der HTML-Quelle behandelt wird, wenn Webabfragedaten in das Arbeitsblatt übernommen werden. Relevant, wenn sourceData True ist"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Wie die Formatierung aus der HTML-Quelle behandelt werden soll, wenn Webabfragedaten in das Arbeitsblatt übernommen werden. Relevant, wenn sourceData True ist.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf die erste vorhandene WebQueryConnection zu (falls vorhanden)
            // Oder erstelle eine neue, indem du eine Datei mit Webverbindungen lädst
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Zeige den anfänglichen HtmlFormat-Wert an
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Setze HtmlFormat auf Rtf (demonstriert Schreibvorgang)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Setze HtmlFormat auf None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Speichere die Arbeitsmappe mit der WebQueryConnection
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

### Siehe auch

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


