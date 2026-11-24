---
title: "WebQueryConnection.IsXl97"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und wird auf true gesetzt, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde. Dies ist ein optionales Attribut, das ignoriert werden kann"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde. Dies ist ein optionales Attribut, das ignoriert werden kann.

```csharp
public bool IsXl97 { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle ein Arbeitsblatt mit einigen Daten, um das Beispiel sinnvoll zu machen
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Erstelle eine Webabfrageverbindung, indem du sie aus einer vorhandenen Datei lädst oder korrekt erstellst
                // Da wir WebQueryConnection nicht direkt erstellen können, greifen wir auf eine vorhandene zu
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Zeige den anfänglichen IsXl97-Wert an
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Setze IsXl97 auf true (da es les- und schreibbar ist)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Setze IsXl97 zurück auf false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Speichere die Arbeitsmappe
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
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


