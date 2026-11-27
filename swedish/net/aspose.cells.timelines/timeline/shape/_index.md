---
title: "Timeline.Shape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Timeline-egenskap. Returnerar TimelineShape-objektet som är associerat med denna Timeline"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

Returnerar [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) objektet som är associerat med denna Timeline.

```csharp
public TimelineShape Shape { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till minimal data som krävs för en tidslinje (datumfält)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // Skapa en pivottabell som kommer att fungera som tidslinjens datakälla
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // Lägg till en tidslinje kopplad till pivottabellen
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // Försök att läsa en 'Shape'-egenskap via reflektion (om den finns i den här versionen)
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

                // Spara arbetsboken för att verifiera att tidslinjeskapandet lyckades
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

### Se även

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


