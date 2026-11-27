---
title: "Slicer.Placement"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Representerar hur ritningsobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett arbetsblad.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället [`Placement`](../../../aspose.cells.drawing/shape/placement/)‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Lägg till en slicer för pivottabellen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Ställ in slicer‑egenskaper inklusive Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Spara arbetsboken
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


