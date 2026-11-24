---
title: "Timeline.WidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Timeline-Eigenschaft. Gibt die Breite der angegebenen Timeline in Pixel zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.timelines/timeline/widthpixel/
---
## Timeline.WidthPixel property

Gibt die Breite der angegebenen Timeline in Pixel zurück oder legt sie fest.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.Width‑Eigenschaft. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen und die Referenz abrufen
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Zeitachse hinzufügen und die Referenz abrufen
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Zeitachsen-Eigenschaften festlegen, einschließlich WidthPixel
            timeline.WidthPixel = 300;
            timeline.HeightPixel = 100;
            timeline.Caption = "Sales Timeline";

            // Speichere die Arbeitsmappe
            workbook.Save("TimelineWidthPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


