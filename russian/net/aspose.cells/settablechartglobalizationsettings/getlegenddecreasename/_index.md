---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает название уменьшения для легенды"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Получает название уменьшения для легенды.

```csharp
public override string GetLegendDecreaseName()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте простые данные для контекста (необязательно)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Создайте диаграмму (необязательно, просто чтобы иметь полную рабочую книгу)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Создайте экземпляр объекта настроек глобализации
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Установите пользовательскую метку уменьшения легенды
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Получите метку, используя GetLegendDecreaseName
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Сохраните рабочую книгу (настройки не привязаны напрямую к диаграмме в этой демонстрации)
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


