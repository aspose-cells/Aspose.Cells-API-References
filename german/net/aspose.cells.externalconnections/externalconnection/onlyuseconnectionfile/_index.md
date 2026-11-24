---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Gibt an, ob die Tabellenkalkulationsanwendung stets und ausschließlich die Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben ist, verwenden soll, wenn die Verbindung aktualisiert wird. Wenn falsch, sollte die Anwendung dem Verfahren folgen, das durch das Attribut reconnectionMethod angegeben ist."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets und ausschließlich die Verbindungsinformationen in der durch das Attribut odcFile angegebenen externen Verbindungsdatei verwenden soll. Wenn false, sollte die Anwendung dem im Attribut reconnectionMethod angegebenen Verfahren folgen.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeigen Sie den aktuellen OnlyUseConnectionFile-Wert an
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Setzen Sie einen neuen OnlyUseConnectionFile-Wert (da er les- und schreibbar ist)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Schalte den Wert um, um die Einstellungsmöglichkeit zu demonstrieren.
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


