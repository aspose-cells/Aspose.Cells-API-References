---
title: "Timeline.WidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Timeline-egenskap. Returnerar eller anger bredden på den angivna tidslinjen i pixlar"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/widthpixel/
---
## Timeline.WidthPixel property

Returnerar eller anger bredden på den angivna tidslinjen, i pixlar.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället Shape.Width-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyWidthPixelDemo
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
            sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell och hämta referensen
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Lägg till tidslinje och hämta referensen
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Ställ in tidslinjeegenskaper inklusive WidthPixel
            timeline.WidthPixel = 300;
            timeline.HeightPixel = 100;
            timeline.Caption = "Sales Timeline";

            // Spara arbetsboken
            workbook.Save("TimelineWidthPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


