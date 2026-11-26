---
title: "Класс ChartGlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartGlobalizationSettings. Представляет настройки глобализации для диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartglobalizationsettings/
---
## ChartGlobalizationSettings class

Представляет настройки глобализации для диаграммы.

```csharp
public class ChartGlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | Получает название заголовка для оси. |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Получает название единицы оси. |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | Получает название заголовка диаграммы. |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | Получает название уменьшения для легенды. |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | Получает название увеличения для легенды. |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | Получает название итога для легенды. |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | Получает название меток "Other" для диаграммы. |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | Получает название серии в диаграмме. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartGlobalizationSettingsDemo
    {
        public static void ChartGlobalizationSettingsExample()
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

            // Продемонстрировать использование методов в ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // Вывести полученные имена в консоль
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // Сохраните книгу
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


