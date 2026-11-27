---
title: "PivotTable.ExternalConnectionDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar den externa anslutningsdatakällan"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

Hämtar den externa anslutningsdatakällan.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället metoden PivotTable.GetSourceDataConnections(). Denna metod kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyExternalConnectionDataSourceDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med extern datakoppling
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa exempeldata
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(2000);

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Hämta den externa anslutningen (skrivskyddad egenskap)
            ExternalConnection connection = pivot.ExternalConnectionDataSource;
            
            if (connection != null)
            {
                Console.WriteLine("Pivot table connection: " + connection.Name);
            }
            else
            {
                Console.WriteLine("No external connection found");
            }
        }
    }
}
```

### Se även

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


