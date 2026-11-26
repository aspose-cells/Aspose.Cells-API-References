---
title: "SettableChartGlobalizationSettings.SetLegendIncreaseName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Устанавливает название увеличения для легенды"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Устанавливает название увеличения для легенды.

```csharp
public void SetLegendIncreaseName(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | локальное зависимое имя |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте минимальные данные для контекста
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Установите пользовательское название увеличения легенды
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Проверьте настройку, получив значение
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Сохраните книгу
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


