---
title: "ExternalConnection.RefreshInternal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.

```csharp
public int RefreshInternal { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Erstelle eine Datenverbindung (unter Verwendung der Basisklasse ExternalConnection).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Setze und zeige die RefreshInternal-Eigenschaft an.
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Ändern Sie das Aktualisierungsintervall
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Speichern Sie die Arbeitsmappe mit den Verbindungseinstellungen
                workbook.Save("RefreshInternalDemo.xlsx");
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


