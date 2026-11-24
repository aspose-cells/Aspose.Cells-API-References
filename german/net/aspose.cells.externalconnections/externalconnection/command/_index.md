---
title: "ExternalConnection.Command"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen

```csharp
public virtual string Command { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Einen Tabellenbereich erstellen
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Eine Pivot-Tabelle erstellen, wobei der Bereich als Quelle verwendet wird
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Die externen Verbindungen abrufen
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Die Command-Eigenschaft der Verbindung anzeigen
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


