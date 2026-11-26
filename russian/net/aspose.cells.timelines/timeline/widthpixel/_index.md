---
title: "Timeline.WidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Timeline. Возвращает или задает ширину указанного таймлайна в пикселях"
type: docs
url: /ru/net/aspose.cells.timelines/timeline/widthpixel/
---
## Timeline.WidthPixel property

Возвращает или задает ширину указанного таймлайна в пикселях.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Shape.Width. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу и получить ссылку
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Добавить временную шкалу и получить ссылку
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Установить свойства временной шкалы, включая WidthPixel
            timeline.WidthPixel = 300;
            timeline.HeightPixel = 100;
            timeline.Caption = "Sales Timeline";

            // Сохраните книгу
            workbook.Save("TimelineWidthPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


