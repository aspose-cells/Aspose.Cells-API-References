---
title: "Slicer.LeftPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Hämtar eller anger den horisontella förskjutningen av slicerformen från dess vänstra kolumn i pixlar"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/leftpixel/
---
## Slicer.LeftPixel property

Hämtar eller anger den horisontella förskjutningen av slicerformen från dess vänstra kolumn, i pixlar.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.Left. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLeftPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);

            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            int slicerIndex = sheet.Slicers.Add(pivotTable, "A10", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            slicer.LeftPixel = 2;

            workbook.Save("SlicerPropertyLeftPixelDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


