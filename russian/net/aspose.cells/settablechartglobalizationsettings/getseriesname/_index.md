---
title: "SettableChartGlobalizationSettings.GetSeriesName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает имя серии в диаграмме"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getseriesname/
---
## SettableChartGlobalizationSettings.GetSeriesName method

Получает название серии в диаграмме.

```csharp
public override string GetSeriesName()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Column A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Column B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Создать и применить настройки глобализации
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetSeriesName("Custom Series Name");
            
            // Настройки глобализации используются при рендеринге/отображении диаграммы,
            // но не назначаются напрямую объекту диаграммы
            // (поскольку у класса Chart нет этого свойства)

            try
            {
                // Получите пользовательское имя серии
                string seriesName = settings.GetSeriesName();
                Console.WriteLine("Series Name: " + seriesName);

                // Сохраните книгу
                workbook.Save("MethodGetSeriesNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


