---
title: "Slicer.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer‑egenskap. Returnerar eller anger bredden på den angivna slicern i punkter"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/width/
---
## Slicer.Width property

Returnerar eller anger bredden på den angivna slicern, i punkter.

```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.WidthPt. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthDemo
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
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till en skivkontroll
            int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Korrekt sätt att lägga till pivottanslutning till slicer
            slicer.AddPivotConnection(pivotTable);

            // Ställ in slicer-egenskaper inklusive bredd
            slicer.Caption = "Fruit Selection";
            slicer.Width = 150; // Setting the width in points
            slicer.Height = 200;

            // Spara arbetsboken
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


