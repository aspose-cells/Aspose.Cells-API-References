---
title: "Timeline.Shape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Timeline. Возвращает объект TimelineShape, связанный с этой Timeline"
type: docs
url: /ru/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

Возвращает объект [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) , связанный с этой Timeline.

```csharp
public TimelineShape Shape { get; }
```

### Примеры

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
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить минимальные данные, необходимые для временной шкалы (поле даты)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // Создать сводную таблицу, которая будет служить источником данных для временной шкалы
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // Добавить временную шкалу, связанную со сводной таблицей
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // Попытаться прочитать свойство 'Shape' через рефлексию (если оно существует в этой версии)
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

                // Сохраните рабочую книгу, чтобы убедиться, что создание шкалы времени успешно
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

### См. также

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


