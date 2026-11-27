---
title: "ExternalConnection.SourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Hämtar eller anger den externa anslutningens DataSource‑typ"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Hämtar eller anger den externa anslutningens DataSource‑typ.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och skapa en pivottabell
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Hämta den externa anslutningen
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Demonstrera SourceType‑egenskapen
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Ändra anslutningsegenskaper
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Skriv ut ändrade egenskaper
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Se även

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


