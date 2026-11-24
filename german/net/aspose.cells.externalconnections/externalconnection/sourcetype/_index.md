---
title: "ExternalConnection.SourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Liest oder setzt den Typ der externen Verbindungs‑Datenquelle"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Ruft den externen Verbindungs‑DataSource‑Typ ab oder legt ihn fest.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Arbeitsblatt hinzu und erstellen Sie eine Pivot‑Tabelle
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Hole die externe Verbindung
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Demonstrieren Sie die SourceType‑Eigenschaft
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Ändern Sie die Verbindungseigenschaften
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Geben Sie die geänderten Eigenschaften aus
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Siehe auch

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


