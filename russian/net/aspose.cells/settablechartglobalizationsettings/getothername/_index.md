---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableChartGlobalizationSettings. Получает имя метки Other для диаграммы"
type: docs
url: /ru/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Получает название меток "Other" для диаграммы.

```csharp
public override string GetOtherName()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте минимальные данные (необязательно, только для полной рабочей книги)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Создайте экземпляр объекта настроек глобализации
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Установите пользовательское имя для метки "Other"
                settings.SetOtherName("Custom Other Label");

                // Получите имя, используя GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Сохраните рабочую книгу (настройки не привязаны напрямую к диаграмме в этой демонстрации)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


