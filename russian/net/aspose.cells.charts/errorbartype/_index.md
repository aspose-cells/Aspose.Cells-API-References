---
title: "Перечисление ErrorBarType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ErrorBarType. Представляет тип количества полос ошибок"
type: docs
url: /ru/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Представляет тип величины полосы ошибок.

```csharp
public enum ErrorBarType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Custom | `0` | Тип значения InnerCustom. |
| FixedValue | `1` | Тип фиксированного значения. |
| Percent | `2` | Тип процента |
| StDev | `3` | Тип стандартного отклонения. |
| StError | `4` | Тип стандартной ошибки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавьте некоторые образцы данных.
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Добавить диаграмму в лист
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Установить свойства линий ошибок для каждой серии в диаграмме
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Сохраните книгу
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


