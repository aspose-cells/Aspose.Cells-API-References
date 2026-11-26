---
title: "Перечисление ChartLineFormattingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ChartLineFormattingType. Представляет тип формата линии диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Представляет тип формата линии диаграммы.

```csharp
public enum ChartLineFormattingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Представляет тип автоматического форматирования. |
| Solid | `1` | Представляет тип сплошного форматирования. |
| None | `2` | Представляет тип отсутствующего форматирования. |
| Gradient | `3` | Градиент |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("A1:B3", true);
            
            // Установите данные категорий
            chart.NSeries.CategoryData = "A1:A3";
            
            // Установите различные типы форматирования линий для серии
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Добавьте другую серию с другим форматированием
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Сохраните книгу
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


