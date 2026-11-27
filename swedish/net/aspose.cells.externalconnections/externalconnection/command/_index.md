---
title: "ExternalConnection.Command"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection property. Strängen som innehåller databaskommandot som ska skickas till data provider‑API:et som kommer att interagera med den externa källan för att hämta data"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

Strängen som innehåller databaskommandot att skicka till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data

```csharp
public virtual string Command { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Skapa ett tabellområde
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Skapa en pivottabell med området som källa
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Hämta de externa anslutningarna
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Visa Command‑egenskapen för anslutningen
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Spara arbetsboken
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


