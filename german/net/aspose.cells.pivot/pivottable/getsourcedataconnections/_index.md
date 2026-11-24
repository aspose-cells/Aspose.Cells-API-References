---
title: "PivotTable.GetSourceDataConnections"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Ruft die externen Verbindungsdatenquellen ab"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Ermittelt die Datenquellen externer Verbindungen.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            
            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Quell-Datenverbindungen abrufen
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Zeige Verbindungsinformationen an
            if (connections.Length > 0)
            {
                ExternalConnection conn = connections[0];
                Console.WriteLine("Connection Name: " + conn.Name);
                Console.WriteLine("Class Type: " + conn.ClassType);
                Console.WriteLine("Source Type: " + conn.SourceType);
                Console.WriteLine("Command: " + conn.Command);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableSourceConnections.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


