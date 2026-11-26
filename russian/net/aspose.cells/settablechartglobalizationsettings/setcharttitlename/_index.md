---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Устанавливает название заголовка диаграммы"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

Устанавливает название заголовка диаграммы.

```csharp
public void SetChartTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // Вызовите SetChartTitleName с пользовательской строкой
                settings.SetChartTitleName("Custom Chart Title");

                // Проверьте настройку, получив значение
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // Сохраните книгу
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


