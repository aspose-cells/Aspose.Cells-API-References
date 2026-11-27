---
title: "Timeline.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Timeline-egenskap. Returnerar eller anger namnet på den angivna tidslinjen"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/name/
---
## Timeline.Name property

Hämtar eller anger namnet på den angivna Timeline

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelinePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för tidslinjen
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            sheet.Cells["A3"].PutValue(DateTime.Now);
            sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
            
            // Lägg till en pivottabell som kommer att användas som datakälla för tidslinjen
            sheet.Cells["C1"].PutValue("Pivot Table");
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till en tidslinje med hjälp av pivottabellen
            int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
            Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Ställ in och demonstrera Name-egenskapen
            timeline.Name = "MyTimeline";
            Console.WriteLine("Timeline name: " + timeline.Name);
        }
    }
}
```

### Se även

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


