---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает имя заголовка диаграммы"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Получает название заголовка диаграммы.

```csharp
public override string GetChartTitleName()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Задайте пользовательское имя заголовка диаграммы
                settings.SetChartTitleName("Custom Chart Title");

                // Получите имя заголовка диаграммы, используя GetChartTitleName
                string chartTitleName = settings.GetChartTitleName();

                // Отобразить результат
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Сохраните книгу
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


