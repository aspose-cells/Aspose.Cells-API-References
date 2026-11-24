---
title: "WebQueryConnection.IsSameSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Kennzeichen, das angibt, ob alle Tabellen innerhalb eines PRE-Blocks mit denselben Breiteneinstellungen wie die erste Zeile geparst werden sollen"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Flag, das angibt, ob alle Tabellen innerhalb eines PRE‑Blocks mit denselben Breiteneinstellungen wie die erste Zeile geparst werden sollen.

```csharp
public bool IsSameSettings { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste vorhandene Webabfrageverbindung zu, falls verfügbar
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Anzeigen des anfänglichen IsSameSettings-Werts
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Setzen Sie IsSameSettings auf true (da es les- und schreibbar ist)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Setzen Sie IsSameSettings zurück auf false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Speichere die Arbeitsmappe
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
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

### Siehe auch

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


