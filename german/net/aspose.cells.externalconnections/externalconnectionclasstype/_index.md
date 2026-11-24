---
title: "Enum ExternalConnectionClassType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionClassType Enum. Stellt den Verbindungstyp dar"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

Stellt den Verbindungstyp dar

```csharp
public enum ExternalConnectionClassType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Database | `0` | ODBC oder OLE DB |
| WebQuery | `1` | Webabfrage |
| TextBased | `2` | Basierend auf Text |
| DataModel | `3` | Datenmodell |
| Unkown | `4` |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionClassTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für die Verbindung hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i - 1);
                worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
            }

            // Erstelle eine Pivot-Tabelle mit den Daten
            int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hole die externe Verbindung und demonstriere Eigenschaften
            ExternalConnection conn = workbook.DataConnections[0];
            
            Console.WriteLine($"Connection Name: {conn.Name}");
            Console.WriteLine($"Class Type: {conn.ClassType}");
            Console.WriteLine($"Source Type: {conn.SourceType}");
            Console.WriteLine($"Command: {conn.Command}");
            Console.WriteLine($"Connection File: {conn.ConnectionFile ?? "null"}");
            Console.WriteLine($"Connection String: {conn.ConnectionString ?? "null"}");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


