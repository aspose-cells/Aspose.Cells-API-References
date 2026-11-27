---
title: "PivotTable.ColumnHeaderCaption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger den anpassade rubriken för kolumnrubriken i PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/columnheadercaption/
---
## PivotTable.ColumnHeaderCaption property

Hämtar och anger den anpassade rubriken för kolumnrubriken i pivottabellen.

```csharp
public string ColumnHeaderCaption { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnHeaderCaptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["A3"].Value = "Bike";
            cells["A4"].Value = "Car";
            cells["A5"].Value = "Car";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Lägg till en pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Ställ in rubriken för kolumnrubriken
            PivotField columnField = pivotTable.ColumnFields[0];
            pivotTable.ColumnHeaderCaption = "Quarter Header";
            
            // Spara arbetsboken
            workbook.Save("PivotTableColumnHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


