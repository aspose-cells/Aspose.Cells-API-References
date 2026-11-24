---
title: "ExternalConnection.KeepAlive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Wahr, wenn die Tabellenkalkulationsanwendung bemüht sein soll, die Verbindung offen zu halten. Wenn falsch, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True, wenn die Tabellenkalkulationsanwendung bemüht sein soll, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen.

```csharp
public bool KeepAlive { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeigen Sie den aktuellen KeepAlive-Wert an
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Schalten Sie den KeepAlive-Wert um, da er les- und schreibbar ist
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("KeepAliveDemo.xlsx");
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


