---
title: "Slicer.NumberOfColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer‑egenskap. Returnerar eller anger antalet kolumner i slicern. Standardvärdet är 1"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

Returnerar eller anger antalet kolumner i slicern. Standardvärdet är 1.

```csharp
public int NumberOfColumns { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Skapa exempeldata för pivottabell
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // Skapa pivottabell – lagra index och hämta sedan PivotTable‑objektet
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Lägg till slicer ansluten till pivottabell
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Konfigurera slicer‑egenskaper
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // Demonstrera NumberOfColumns‑egenskapen
            slicer.NumberOfColumns = 2;

            // Spara arbetsboken
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


