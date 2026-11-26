---
title: "Перечисление TickMarkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.TickMarkType. Представляет тип деления для указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Представляет тип деления для указанной оси.

```csharp
public enum TickMarkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Cross | `0` | Тип деления – Cross. |
| Inside | `1` | Тип деления – Inside. |
| None | `2` | Тип деления – None. |
| Outside | `3` | Тип деления – Outside |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте NSeries (источник данных диаграммы) к диаграмме, охватывающий ячейки от "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Получите доступ к оси значений диаграммы
            Axis valueAxis = chart.ValueAxis;

            // Установите тип основных делений в Cross
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Установите тип вспомогательных делений в Inside
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Установите максимальное значение оси значений
            valueAxis.MaxValue = 200;

            // Установите минимальное значение оси значений
            valueAxis.MinValue = 0;

            // Установите основной интервал
            valueAxis.MajorUnit = 25;

            // Сохраните книгу
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


