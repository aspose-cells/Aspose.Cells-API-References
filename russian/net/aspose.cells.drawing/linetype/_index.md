---
title: "Перечисление LineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.LineType. Перечисляет тип границы изображения или линии диаграммы"
type: docs
url: /ru/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Перечисляет тип границы [`Picture`](../picture/) или линии [`Chart`](../../aspose.cells.charts/chart/).

```csharp
public enum LineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DarkGray | `6` | Представляет темно-серую линию. |
| Dash | `1` | Представляет пунктирную линию. |
| DashDot | `3` | Представляет линию штрих-точка |
| DashDotDot | `4` | Представляет линию штрих-точка-точка. |
| Dot | `2` | Представляет точечную линию. |
| LightGray | `8` | Представляет светло-серую линию. |
| MediumGray | `7` | Представляет средне-серую линию. |
| Solid | `0` | Представляет сплошную линию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // Получить доступ к основной оси категорий
            Axis categoryAxis = chart.CategoryAxis;

            // Установите тип линии для осевой линии
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Установите цвет осевой линии
            categoryAxis.AxisLine.Color = Color.Blue;

            // Получить доступ к основной оси значений
            Axis valueAxis = chart.ValueAxis;

            // Установите тип линии для основных линий сетки
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Установите цвет основных линий сетки
            valueAxis.MajorGridLines.Color = Color.Red;

            // Сохраните книгу
            workbook.Save("LineTypeExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


