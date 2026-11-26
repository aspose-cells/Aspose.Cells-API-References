---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Устанавливает имя Decrease для легенды"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Устанавливает название уменьшения для легенды.

```csharp
public void SetLegendDecreaseName(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | локальное зависимое имя |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Создать настройки глобализации
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Вызовите SetLegendDecreaseName с пользовательской строкой
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // У класса Chart нет свойства ChartGlobalizationSettings,
                // поэтому нам нужно использовать объект настроек напрямую там, где это необходимо
                // (Примечание: в реальном использовании вам потребуется найти, где применяются эти настройки)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


