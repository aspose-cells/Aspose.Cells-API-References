---
title: "Перечисление QuartileCalculationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.QuartileCalculationType. Представляет методы расчёта квартилей"
type: docs
url: /ru/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Представляет методы расчёта квартилей.

```csharp
public enum QuartileCalculationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Exclusive | `0` | Расчёт квартилей включает медиану при разделении набора данных на квартильные группы. |
| Inclusive | `1` | Расчёт квартилей исключает медиану при разделении набора данных на квартильные группы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию к диаграмме
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Получите доступ к свойствам макета серии
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Установите тип расчёта квартилей
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Сохраните книгу
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


