---
title: "ExternalConnection.ClassType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Hämtar typen av detta ExternalConnection‑objekt"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Hämtar typen av detta [`ExternalConnection`](../) objekt.

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Skapa en pivottabell med Data Model‑anslutning
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hämta den externa anslutningen och demonstrera ClassType‑egenskapen
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // Spara arbetsboken
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


