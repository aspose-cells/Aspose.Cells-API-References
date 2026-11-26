---
title: "Перечисление GradientStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Представляет стиль градиентного затенения"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Представляет стиль затенения градиента.

```csharp
public enum GradientStyleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DiagonalDown | `0` | Стиль затенения по диагонали вниз |
| DiagonalUp | `1` | Стиль затенения по диагонали вверх |
| FromCenter | `2` | Стиль затенения от центра |
| FromCorner | `3` | Стиль затенения от угла |
| Horizontal | `4` | Горизонтальный стиль затенения |
| Vertical | `5` | Вертикальный стиль затенения |
| Unknown | `6` | Неизвестный стиль затенения. Только для стиля затенения (который не относится ни к одному члену GradientStyleType) в файле шаблона. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
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

            // Установить двухцветную градиентную заливку со стилем DiagonalDown
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Вывести используемый стиль градиента
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Сохраните книгу
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


