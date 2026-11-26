---
title: "ChartGlobalizationSettings.GetSeriesName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Возвращает название Series в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getseriesname/
---
## ChartGlobalizationSettings.GetSeriesName method

Получает название серии в диаграмме.

```csharp
public virtual string GetSeriesName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавьте диаграмму и задайте данные
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Создайте настройки глобализации и получите имя серии
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string seriesName = globalizationSettings.GetSeriesName();

            // Вывести результат.
            Console.WriteLine("Series Name: " + seriesName);

            // Сохраните книгу
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### См. также

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


