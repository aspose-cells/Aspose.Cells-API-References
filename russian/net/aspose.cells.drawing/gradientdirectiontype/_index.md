---
title: "Перечисление GradientDirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.GradientDirectionType. Представляет все типы направлений градиента"
type: docs
url: /ru/net/aspose.cells.drawing/gradientdirectiontype/
---
## GradientDirectionType enumeration

Представляет все типы направлений градиента.

```csharp
public enum GradientDirectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Неизвестно |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientDirectionTypeDemo
    {
        public static void GradientDirectionTypeExample()
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

            // Получить доступ к области построения диаграммы
            PlotArea plotArea = chart.PlotArea;

            // Получить доступ к формату заливки области построения
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Установить двухцветную заливку градиентом с определённым направлением
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Вывести тип направления градиента
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Сохраните книгу
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


