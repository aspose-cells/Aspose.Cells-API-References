---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Flag, das angibt, dass XML-Quelldaten anstelle der HTML-Tabelle selbst importiert werden sollen"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

Flag, das angibt, dass XML-Quelldaten importiert werden sollen anstelle der HTML‑Tabelle selbst.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf eine vorhandene Webabfrageverbindung zu oder erstelle eine über die richtige Initialisierung
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Zeige den anfänglichen IsXmlSourceData-Wert an
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Setze IsXmlSourceData auf true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Setze IsXmlSourceData zurück auf false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Speichere die Arbeitsmappe
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

### Siehe auch

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


