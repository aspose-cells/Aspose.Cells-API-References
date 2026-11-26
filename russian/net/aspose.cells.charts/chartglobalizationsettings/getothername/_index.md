---
title: "ChartGlobalizationSettings.GetOtherName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Возвращает название меток Other для диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getothername/
---
## ChartGlobalizationSettings.GetOtherName method

Получает название меток "Other" для диаграммы.

```csharp
public virtual string GetOtherName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetOtherNameDemo
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
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Создать настройки глобализации и получить название Other
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string otherName = globalizationSettings.GetOtherName();

            // Вывести результат.
            Console.WriteLine("Other Name: " + otherName);

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


