---
title: "Slicer.Title"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Anger titeln på det aktuella Slicer-objektet"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/title/
---
## Slicer.Title property

Anger titeln på det aktuella Slicer-objektet.

```csharp
[Obsolete("Use Shape.Title property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string Title { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället [`Title`](../../../aspose.cells.drawing/shape/title/) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTitleDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C1", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.CalculateData();

            // Lägg till skärmningskontrollen
            SlicerCollection slicers = worksheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];
            
            // Ange slicer-titel
            slicer.Title = "Fruit Selection Slicer";
            
            // Spara arbetsboken
            workbook.Save("SlicerTitleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


