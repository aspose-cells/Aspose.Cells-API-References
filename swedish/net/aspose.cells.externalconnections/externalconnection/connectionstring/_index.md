---
title: "ExternalConnection.ConnectionString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla.

```csharp
public virtual string ConnectionString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Hämta dataanslutningarna
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Visa anslutningssträngen om den finns
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // Spara arbetsboken
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### Se även

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


