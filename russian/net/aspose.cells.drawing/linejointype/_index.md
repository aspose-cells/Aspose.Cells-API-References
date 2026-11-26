---
title: "Перечисление LineJoinType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.LineJoinType. Представляет стили соединения линии"
type: docs
url: /ru/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Представляет стили соединения линии.

```csharp
public enum LineJoinType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Round | `0` | Скругленное соединение |
| Bevel | `1` | Фаска соединения |
| Miter | `2` | Угловое соединение |
| None | `3` | Нет соединения |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Получить доступ к основной оси значений
            Axis valueAxis = chart.ValueAxis;

            // Получить доступ к формату линий основных сеток
            Line majorGridLines = valueAxis.MajorGridLines;

            // Установить тип соединения линии
            majorGridLines.JoinType = LineJoinType.Round;

            // Вывести тип соединения
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Сохраните книгу
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


