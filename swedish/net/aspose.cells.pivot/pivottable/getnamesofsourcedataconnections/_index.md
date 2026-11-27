---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Hämtar namnen på externa källans datakopplingar"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Hämtar namnen på externa datakällans anslutningar.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // Skapa pivottabell och hämta referens
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Hämta källdataanslutningar
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // Skriv ut anslutningsinformationen
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


