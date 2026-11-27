---
title: "Enum ExternalConnectionClassType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionClassType enum. Representerar anslutningstypen"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

Representerar anslutningstypen

```csharp
public enum ExternalConnectionClassType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Database | `0` | ODBC eller OLE DB |
| WebQuery | `1` | Web‑fråga |
| TextBased | `2` | Baserat på text |
| DataModel | `3` | Datamodell |
| Unkown | `4` |  |

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för anslutningen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i - 1);
                worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
            }

            // Skapa en pivottabell med data
            int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hämta den externa anslutningen och demonstrera egenskaper
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

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


