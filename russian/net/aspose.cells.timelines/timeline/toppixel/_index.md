---
title: "Timeline.TopPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Timeline. Возвращает или задает вертикальное смещение формы временной шкалы от её верхней строки в пикселях"
type: docs
url: /ru/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

Возвращает или задает вертикальное смещение формы временной шкалы от её верхней строки, в пикселях.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Top. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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
            // Создайте новую книгу и получите первый лист
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить примерными данными
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Добавить PivotTable
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Добавить Timeline
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // Установить свойства Timeline, включая TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // Сохраните книгу
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


