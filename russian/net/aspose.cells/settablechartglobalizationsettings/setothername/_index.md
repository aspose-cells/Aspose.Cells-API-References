---
title: "SettableChartGlobalizationSettings.SetOtherName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Устанавливает имя остальных меток для диаграммы"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Устанавливает название меток "Other" для диаграммы.

```csharp
public void SetOtherName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте минимальные данные для контекста
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Создать экземпляр SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Установите пользовательское имя для метки "Other"
                settings.SetOtherName("Miscellaneous Items");

                // Проверьте настройку, получив значение
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Сохраните книгу
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


