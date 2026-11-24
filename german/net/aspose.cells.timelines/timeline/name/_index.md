---
title: "Timeline.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Timeline-Eigenschaft. Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.timelines/timeline/name/
---
## Timeline.Name property

Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest

```csharp
public string Name { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für die Timeline hinzufügen
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            sheet.Cells["A3"].PutValue(DateTime.Now);
            sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
            
            // Pivot-Tabelle hinzufügen, die als Datenquelle für die Timeline verwendet wird
            sheet.Cells["C1"].PutValue("Pivot Table");
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Eine Timeline mithilfe der Pivot-Tabelle hinzufügen
            int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
            Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Setzen und demonstrieren Sie die Name‑Eigenschaft
            timeline.Name = "MyTimeline";
            Console.WriteLine("Timeline name: " + timeline.Name);
        }
    }
}
```

### Siehe auch

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


