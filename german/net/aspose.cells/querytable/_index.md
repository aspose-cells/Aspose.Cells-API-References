---
title: "Klasse QueryTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTable Klasse. Stellt QueryTable-Informationen dar."
type: docs
url: /de/net/aspose.cells/querytable/
---
## QueryTable class

Stellt QueryTable-Informationen dar.

```csharp
public class QueryTable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Liest die Verbindungs-ID der Abfrage‑Tabelle. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Liest die zugehörige externe Verbindung. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Liest den Namen der Abfrage‑Tabelle. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Gibt die PreserveFormatting des Objekts zurück oder setzt sie. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Liest den Bereich des Ergebnisses. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu, um eine Abfrage‑Tabelle zu erstellen (simuliert externe Daten).
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Prüfe, ob im Arbeitsblatt Abfrage‑Tabellen vorhanden sind.
            if (worksheet.QueryTables.Count > 0)
            {
                // Hole die erste Abfrage‑Tabelle.
                QueryTable qt = worksheet.QueryTables[0];
                
                // Zeige die Eigenschaften der Abfrage‑Tabelle an.
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Ändere einige Eigenschaften.
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


