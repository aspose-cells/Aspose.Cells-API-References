---
title: "Перечисление LegendPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.LegendPositionType. Перечисляет типы положения легенды"
type: docs
url: /ru/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Перечисляет типы положения легенды.

```csharp
public enum LegendPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Bottom | `0` | Отображает легенду в нижней части области построения диаграммы. |
| Corner | `1` | Отображает легенду в углу области построения диаграммы. |
| Left | `4` | Отображает легенду слева от области построения диаграммы. |
| NotDocked | `7` | Указывает, что легенда не закреплена. |
| Right | `3` | Отображает легенду справа от области построения диаграммы. |
| Top | `2` | Отображает легенду в верхней части области построения диаграммы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Добавить столбчатую диаграмму на лист
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Получите доступ к легенде диаграммы
            Legend legend = chart.Legend;

            // Установите положение легенды слева от диаграммы
            legend.Position = LegendPositionType.Left;

            // Установите дополнительные свойства для легенды
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Сохраните книгу
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


