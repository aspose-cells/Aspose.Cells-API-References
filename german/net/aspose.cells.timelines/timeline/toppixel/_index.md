---
title: "Timeline.TopPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Timeline-Eigenschaft. Gibt den vertikalen Versatz der Timeline‑Form von ihrer oberen Zeile in Pixel zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

Gibt den vertikalen Versatz der Timeline‑Form von ihrer oberen Zeile in Pixel zurück oder legt ihn fest.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Shape.Top‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten befüllen
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // PivotTable hinzufügen
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Timeline hinzufügen
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // Timeline‑Eigenschaften festlegen, einschließlich TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // Speichere die Arbeitsmappe
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


