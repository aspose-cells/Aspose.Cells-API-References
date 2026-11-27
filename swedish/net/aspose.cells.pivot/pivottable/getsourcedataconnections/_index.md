---
title: "PivotTable.GetSourceDataConnections"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Hämtar de externa anslutningsdatakällorna"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Hämtar de externa anslutningsdatakällorna.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            
            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Hämta källdataanslutningar
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Visa anslutningsinformation
            if (connections.Length > 0)
            {
                ExternalConnection conn = connections[0];
                Console.WriteLine("Connection Name: " + conn.Name);
                Console.WriteLine("Class Type: " + conn.ClassType);
                Console.WriteLine("Source Type: " + conn.SourceType);
                Console.WriteLine("Command: " + conn.Command);
            }
            
            // Spara arbetsboken
            workbook.Save("PivotTableSourceConnections.xlsx");
        }
    }
}
```

### Se även

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


