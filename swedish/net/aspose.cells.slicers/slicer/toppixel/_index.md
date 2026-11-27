---
title: "Slicer.TopPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer‑egenskap. Returnerar eller anger det vertikala avståndet för slicer‑formen från dess översta rad i pixlar"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

Returnerar eller anger det vertikala avståndet för slicer‑formen från dess översta rad, i pixlar.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället Shape.Top-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTopPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Skapa pivottabell och hämta dess index
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Lägg till slicer och hämta dess index
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Ställ in TopPixel‑egenskapen
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


