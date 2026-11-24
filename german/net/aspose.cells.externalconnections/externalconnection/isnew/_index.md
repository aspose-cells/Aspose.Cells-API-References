---
title: "ExternalConnection.IsNew"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. True, wenn die Verbindung zum ersten Mal noch nicht aktualisiert wurde, sonst false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist.

```csharp
public bool IsNew { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (neu erstellte Verbindungen sind typischerweise \"IsNew\")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeigen Sie den anfänglichen IsNew-Wert an
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Da IsNew les- und schreibbar ist, demonstrieren Sie das Setzen
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("IsNewDemo.xlsx");
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


