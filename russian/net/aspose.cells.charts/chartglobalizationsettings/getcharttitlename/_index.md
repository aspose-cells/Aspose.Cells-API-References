---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Получает имя заголовка диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

Получает название заголовка диаграммы.

```csharp
public virtual string GetChartTitleName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Создать экземпляр ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Продемонстрируйте использование метода GetChartTitleName
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

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


