---
title: "Перечисление ChartMarkerType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ChartMarkerType. Представляет стиль маркера в линейной диаграмме, точечной диаграмме или радиальной диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Представляет стиль маркера в линейной, точечной или радиальной диаграмме.

```csharp
public enum ChartMarkerType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Автоматические маркеры. |
| Circle | `1` | Круговые маркеры. |
| Dash | `2` | Маркер длинного столбца |
| Diamond | `3` | Маркер в виде ромба. |
| Dot | `4` | Маркер короткого столбца. |
| None | `5` | Без маркеров. |
| SquarePlus | `6` | Квадратные маркеры с плюсом. |
| Square | `7` | Квадратные маркеры. |
| SquareStar | `8` | Квадратные маркеры со звездочкой. |
| Triangle | `9` | Треугольные маркеры. |
| SquareX | `10` | Квадратные маркеры с крестом. |
| Picture | `11` | Изображение |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию данных к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к маркеру первой серии
            Marker marker = chart.NSeries[0].Marker;

            // Установить стиль маркера
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Установить размер маркера
            marker.MarkerSize = 10;

            // Установить цвета переднего плана и фона маркера
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Сохраните книгу
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


