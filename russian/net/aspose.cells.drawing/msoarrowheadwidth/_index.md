---
title: "Перечисление MsoArrowheadWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoArrowheadWidth. Перечисляет ширину конца линии границы фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Перечисляет ширину конца линии границы фигуры.

```csharp
public enum MsoArrowheadWidth
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Narrow | `0` | Короткая ширина конца линии. |
| Medium | `1` | Средняя ширина конца линии. |
| Wide | `2` | Широкая ширина конца линии. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
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

            // Создать форму линии для диаграммы
            Line line = chart.Line;

            // Установить стили и толщины наконечников стрелок
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Вывести стили и толщины наконечников стрелок
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Сохраните книгу
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


