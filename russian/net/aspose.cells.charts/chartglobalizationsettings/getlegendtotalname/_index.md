---
title: "ChartGlobalizationSettings.GetLegendTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Получает имя общего значения для легенды"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

Получает название итога для легенды.

```csharp
public virtual string GetLegendTotalName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendTotalNameDemo
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

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Создайте настройки глобализации и получите имя общего значения легенды
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendTotalName = globalizationSettings.GetLegendTotalName();

            // Вывести результат.
            Console.WriteLine("Legend Total Name: " + legendTotalName);

            // Сохранить книгу
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


