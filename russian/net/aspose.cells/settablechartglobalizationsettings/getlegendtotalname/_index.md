---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает имя итога для легенды"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Получает название итога для легенды.

```csharp
public override string GetLegendTotalName()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Сначала задайте пользовательское имя итога легенды
                settings.SetLegendTotalName("Custom Total Label");

                // Вызовите метод GetLegendTotalName, чтобы получить значение
                string legendTotalName = settings.GetLegendTotalName();

                // Отобразить результат
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Сохраните книгу
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


