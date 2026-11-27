---
title: "PivotTable.PivotTableStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Hämtar eller anger stilnamn för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pivottablestylename/
---
## PivotTable.PivotTableStyleName property

Hämtar eller anger stilnamnet för pivottabellen.

```csharp
public string PivotTableStyleName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Data;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Applicera en inbyggd pivottabellstil
            pivotTable.PivotTableStyleName = "PivotStyleLight16";
            
            // Spara arbetsboken
            workbook.Save("PivotTableStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


