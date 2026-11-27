---
title: "Slicer.LockedPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer‑egenskap. Anger om den angivna slicern kan flyttas eller ändras i storlek via användargränssnittet"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Anger om den angivna slicern kan flyttas eller ändras i storlek via användargränssnittet.

```csharp
public bool LockedPosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
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

            // Skapa pivottabellsamling
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Skapa en pivottabell
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Skapa slicer-samling
            SlicerCollection slicers = worksheet.Slicers;
            
            // Lägg till en slicer för pivottabellen
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Ange skivkontrollens egenskaper
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Demonstrera egenskapen LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Ändra LockedPosition till false för att tillåta rörelse
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Spara arbetsboken
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


