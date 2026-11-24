---
title: "WebQueryConnection.IsTextDates"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Kennzeichen, das angibt, ob Datumswerte als Text statt als Datum in Zellen des Arbeitsblatts importiert werden sollen"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Flag, das angibt, ob Daten als Text statt als Datum in Zellen des Arbeitsblatts importiert werden sollen.

```csharp
public bool IsTextDates { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Erstellen Sie eine Webabfrageverbindung, indem Sie sie aus einer vorhandenen Datei laden
                // oder indem Sie eine vorhandene Verbindung verwenden
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Anzeigen des anfänglichen IsTextDates-Werts
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Setzen Sie IsTextDates auf true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Setzen Sie IsTextDates zurück auf false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Speichere die Arbeitsmappe mit der WebQueryConnection
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
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


