---
title: "WebQueryConnection.IsXml"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. true, wenn die Webabfragequelle XML statt HTML ist, sonst false"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true, wenn die Webabfragequelle XML (statt HTML) ist, andernfalls false.

```csharp
public bool IsXml { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf die erste Datenverbindung zu (angenommen, es ist eine WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Zeige den anfänglichen IsXml-Wert an
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // Setze IsXml auf true (da es les- und schreibbar ist)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // Setze IsXml zurück auf false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // Speichere die Arbeitsmappe
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

### Siehe auch

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


