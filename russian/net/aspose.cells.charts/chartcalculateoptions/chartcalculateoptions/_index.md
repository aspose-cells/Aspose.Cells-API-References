---
title: "ChartCalculateOptions.ChartCalculateOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ChartCalculateOptions. Создаёт параметры для расчёта диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartcalculateoptions/chartcalculateoptions/
---
## ChartCalculateOptions constructor

Создаёт параметры расчёта диаграммы.

```csharp
public ChartCalculateOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Создать ChartCalculateOptions с помощью конструктора
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            
            // Пересчитать диаграмму с параметрами
            chart.Calculate(calculateOptions);

            // Сохраните книгу
            workbook.Save("ChartCalculateOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


