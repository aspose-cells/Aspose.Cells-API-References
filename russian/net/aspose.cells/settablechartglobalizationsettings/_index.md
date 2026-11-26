---
title: "Класс SettableChartGlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SettableChartGlobalizationSettings. Реализация PivotGlobalizationSettings, которая позволяет пользователю задавать/изменять предопределённые тексты"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Реализация PivotGlobalizationSettings, позволяющая пользователю задавать/изменять предопределённые тексты.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Получает название заголовка для оси. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Получает название единицы оси. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Получает название заголовка диаграммы. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Получает название уменьшения для легенды. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Получает название увеличения для легенды. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Получает название итога для легенды. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Получает название меток "Other" для диаграммы. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Получает название серии в диаграмме. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Устанавливает название заголовка для оси. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Устанавливает название единицы оси. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Устанавливает название заголовка диаграммы. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Устанавливает название уменьшения для легенды. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Устанавливает название увеличения для легенды. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Устанавливает название итога для легенды. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Устанавливает название меток "Other" для диаграммы. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Устанавливает название серии в диаграмме. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Установить пользовательские настройки глобализации
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Создать пользовательскую реализацию GlobalizationSettings
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Создать простую диаграмму для демонстрации настроек
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // Реализовать необходимые методы GlobalizationSettings здесь
            // делегируют к экземпляру SettableChartGlobalizationSettings
        }
    }
}
```

### См. также

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


