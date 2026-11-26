---
title: "ChartGlobalizationSettings.GetAxisTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartGlobalizationSettings. Получает имя заголовка для оси"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/getaxistitlename/
---
## ChartGlobalizationSettings.GetAxisTitleName method

Получает название заголовка для оси.

```csharp
public virtual string GetAxisTitleName()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
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

            // Создайте настройки глобализации и получите имя заголовка оси
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string axisTitleName = globalizationSettings.GetAxisTitleName();

            // Установите заголовок оси
            chart.ValueAxis.Title.Text = axisTitleName;
            chart.CategoryAxis.Title.Text = axisTitleName;

            // Выведите имя заголовка оси
            Console.WriteLine("Axis Title Name: " + axisTitleName);

            // Сохраните книгу
            workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


