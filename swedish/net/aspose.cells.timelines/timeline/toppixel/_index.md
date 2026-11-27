---
title: "Timeline.TopPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Timeline-egenskap. Returnerar eller anger det vertikala offsetet för tidslinjeformen från dess översta rad i pixlar"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

Returnerar eller anger det vertikala offsetet för tidslinjeformen, i pixlar.

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
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyTopPixelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i exempeldata
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Lägg till PivotTable
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Lägg till Timeline
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // Ställ in Timeline-egenskaper inklusive TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // Spara arbetsboken
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


