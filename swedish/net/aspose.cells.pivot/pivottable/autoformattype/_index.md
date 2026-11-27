---
title: "PivotTable.AutoFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger den automatiska formattypen för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Hämtar och anger automatisk formattyp för PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutoFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Chair");
            worksheet.Cells["C4"].PutValue(150);
            
            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
            
            // Demonstrera AutoFormatType-egenskapen
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
            
            // Spara arbetsboken
            workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


