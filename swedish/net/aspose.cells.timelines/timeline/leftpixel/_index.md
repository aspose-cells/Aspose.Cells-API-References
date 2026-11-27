---
title: "Timeline.LeftPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen Timeline. Returnerar eller anger det horisontella avståndet för tidslinjens form från dess vänstra kolumn i pixlar"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/leftpixel/
---
## Timeline.LeftPixel property

Returnerar eller anger det horisontella avståndet för tidslinjens form från dess vänstra kolumn, i pixlar.

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
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyLeftPixelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();

            // Lägg till tidslinjen och hämta den från samlingen
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Demonstrera LeftPixel‑egenskapen
            timeline.LeftPixel = 150;
            timeline.TopPixel = 50;
            timeline.WidthPixel = 200;
            timeline.HeightPixel = 80;

            // Spara arbetsbok
            workbook.Save("TimelineLeftPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


