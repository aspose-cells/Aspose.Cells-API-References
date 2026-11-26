---
title: "ChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Получает имя уменьшения для легенды"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/
---
## ChartGlobalizationSettings.GetLegendDecreaseName method

Получает название уменьшения для легенды.

```csharp
public virtual string GetLegendDecreaseName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Создайте настройки глобализации и получите имя уменьшения легенды
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();

            // Вывести результат.
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

            // Сохраните книгу
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


