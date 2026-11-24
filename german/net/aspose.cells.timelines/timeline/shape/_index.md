---
title: "Timeline.Shape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Timeline‑Eigenschaft. Gibt das mit diesem Timeline verknüpfte TimelineShape‑Objekt zurück"
type: docs
url: /de/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

Gibt das [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) Objekt zurück, das mit diesem Timeline verknüpft ist.

```csharp
public TimelineShape Shape { get; }
```

### Beispiele

```csharp
using System;
using System.Reflection;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyShapeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie die minimalen für eine Timeline erforderlichen Daten hinzu (Datumsfeld)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // Erstellen Sie eine PivotTable, die als Datenquelle für die Timeline dient
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // Fügen Sie eine Timeline hinzu, die mit der PivotTable verknüpft ist
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // Versuchen Sie, die 'Shape'-Eigenschaft per Reflexion zu lesen (falls sie in dieser Version existiert)
                PropertyInfo shapeProp = typeof(Timeline).GetProperty("Shape", BindingFlags.Public | BindingFlags.Instance);
                if (shapeProp != null)
                {
                    object shapeValue = shapeProp.GetValue(timeline);
                    Console.WriteLine("Shape property value: " + (shapeValue ?? "null"));
                }
                else
                {
                    Console.WriteLine("The Timeline class does not expose a 'Shape' property in this version.");
                }

                // Speichern Sie die Arbeitsmappe, um zu überprüfen, ob die Erstellung der Timeline erfolgreich war
                workbook.Save("TimelineShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


