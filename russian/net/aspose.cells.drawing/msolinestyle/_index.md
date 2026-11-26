---
title: "Перечисление MsoLineStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoLineStyle. Представляет стиль рисуемых линий"
type: docs
url: /ru/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Представляет стиль линий рисования.

```csharp
public enum MsoLineStyle
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Single | `0` | Одна линия (ширины lineWidth) |
| ThickBetweenThin | `1` | Три линии: тонкая, толстая, тонкая |
| ThinThick | `2` | Две линии, одна тонкая, одна толстая |
| ThickThin | `3` | Две линии, одна толстая, одна тонкая |
| ThinThin | `4` | Две линии одинаковой ширины |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
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

            // Установить стиль линии для основной оси категорий
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Вывести стиль линии
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Сохраните книгу
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


