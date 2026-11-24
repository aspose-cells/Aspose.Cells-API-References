---
title: "ExternalConnection.SaveData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Wahr, wenn die über die Verbindung abgerufenen externen Daten, die eine Tabelle füllen, mit der Arbeitsmappe gespeichert werden sollen, andernfalls falsch"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit dem Arbeitsbuch gespeichert werden sollen; andernfalls false.

```csharp
public bool SaveData { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Aktuellen SaveData-Wert anzeigen
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Demonstriere das Setzen der Eigenschaft (da sie les- und schreibbar ist).
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("SaveDataDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


