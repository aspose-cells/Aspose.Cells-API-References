---
title: "WebQueryConnection.IsConsecutive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Kennzeichen, das angibt, ob aufeinanderfolgende Trennzeichen als ein einziges Trennzeichen behandelt werden sollen"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Flag, das angibt, ob aufeinanderfolgende Trennzeichen als ein einzelnes Trennzeichen behandelt werden sollen.

```csharp
public bool IsConsecutive { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstellen Sie eine Webabfrageverbindung, indem Sie die erste Verbindung verwenden
            // (unter der Annahme, dass mindestens eine Verbindung verfügbar ist)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Anzeigen des anfänglichen IsConsecutive-Werts (Standard)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Setzen Sie IsConsecutive auf true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Setze IsConsecutive zurück auf false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Speichere die Arbeitsmappe mit der WebQueryConnection
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


