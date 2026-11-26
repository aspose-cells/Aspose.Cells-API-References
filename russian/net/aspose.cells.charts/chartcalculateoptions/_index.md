---
title: "Класс ChartCalculateOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartCalculateOptions. Представляет параметры расчёта диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Представляет параметры расчёта диаграммы.

```csharp
public class ChartCalculateOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Создаёт параметры расчёта диаграммы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Обновлять ли все точки данных при выполнении расчёта диаграммы. По умолчанию: False. Если вы хотите получить значение каждой отдельной точки данных в диаграмме, установите значение true. Если этот параметр установлен в True, новые точки данных могут быть созданы при расчёте диаграммы. Это может увеличить размер файла Excel. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Создать экземпляр ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Выполнить расчёт диаграммы с указанными параметрами
            chart.Calculate(options);

            // Сохраните книгу
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


