---
title: "ExternalConnection.CommandType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection property. Anger OLE DB‑kommandotypen. 1. Frågan anger ett kubnamn 2. Frågan anger ett SQL‑uttryck 3. Frågan anger ett tabellnamn 4. Frågan anger att standardinformation har givits och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webb‑baserad List Data Provider"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webbaserad List Data Provider.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Hämta den externa anslutningen
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Demonstrera CommandType‑egenskapen
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // Ändra och visa CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Spara arbetsboken
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


