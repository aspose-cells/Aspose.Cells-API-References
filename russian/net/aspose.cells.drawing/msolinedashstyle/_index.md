---
title: "Перечисление MsoLineDashStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoLineDashStyle. Представляет стиль пунктирных линий"
type: docs
url: /ru/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Представляет стиль пунктирных линий.

```csharp
public enum MsoLineDashStyle
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Dash | `0` | Представляет пунктирную линию. |
| DashDot | `1` | Представляет линию тире-точка. |
| DashDotDot | `2` | Представляет линию штрих-точка-точка. |
| DashLongDash | `3` | Представляет линию длинное тире-короткое тире. |
| DashLongDashDot | `4` | Представляет линию длинное тире-короткое тире-точка. |
| RoundDot | `5` | Представляет линию с круглыми точками. |
| Solid | `6` | Представляет сплошную линию. |
| SquareDot | `7` | Представляет линию с квадратными точками. |
| Custom | `8` | Пользовательский стиль пунктиров. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Установить стиль пунктиров основных линий сетки
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Установить стиль пунктиров вспомогательных линий сетки
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Сохраните книгу
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


