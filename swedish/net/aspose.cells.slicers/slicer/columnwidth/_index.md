---
title: "Slicer.ColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Returnerar eller anger bredden på varje kolumn i slicern i enheten punkter"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/columnwidth/
---
## Slicer.ColumnWidth property

Returnerar eller anger bredden på varje kolumn i slicern i enheter av punkter.

```csharp
public double ColumnWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            
            // Lägg till pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Lägg till skärmningskontrollen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Ställ in kolumnbredd i punkter
            slicer.ColumnWidth = 80;
            
            // Spara arbetsboken
            workbook.Save("SlicerColumnWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


