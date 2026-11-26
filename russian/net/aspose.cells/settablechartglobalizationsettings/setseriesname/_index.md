---
title: "SettableChartGlobalizationSettings.SetSeriesName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Устанавливает название серии в диаграмме"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Устанавливает название серии в диаграмме.

```csharp
public void SetSeriesName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте минимальные данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Установите пользовательское название серии, используя SetSeriesName со строковым параметром
                settings.SetSeriesName("Custom Series Label");

                // Проверьте настройку, получив название серии
                string seriesName = settings.GetSeriesName();
                Console.WriteLine($"Series name set to: {seriesName}");

                // Сохраните книгу
                workbook.Save("SetSeriesNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetSeriesName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


