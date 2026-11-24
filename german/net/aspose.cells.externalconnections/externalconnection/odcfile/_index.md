---
title: "ExternalConnection.OdcFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection‑Eigenschaft. Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung während eines Versuchs, Daten zu aktualisieren, und reconnectionMethod1 fehlschlägt, versucht die Tabellenkalkulationsanwendung es erneut mit Informationen aus der externen Verbindungsdatei anstelle des in der Arbeitsmappe eingebetteten Verbindungsobjekts."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei anstelle des im Arbeitsbuch eingebetteten Verbindungsobjekts zu verwenden.

```csharp
public string OdcFile { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Anzeigen des aktuellen OdcFile-Werts
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Setzen Sie einen neuen OdcFile-Wert (da er les‑ und schreibbar ist)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Löschen Sie den OdcFile-Wert
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("OdcFileDemo.xlsx");
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


