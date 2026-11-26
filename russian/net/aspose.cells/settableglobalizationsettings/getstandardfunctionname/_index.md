---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает стандартное имя функции в соответствии с заданным именем функции, зависящим от локали"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Получает стандартное название функции в соответствии с заданным названием функции, зависящим от локали.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | String | Имя функции, зависящее от локали. Локаль была указана в Workbook, для которого используются эти настройки. |

### Возвращаемое значение

Стандартное имя функции (локаль en-US).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установить сопоставление локального имени функции
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызвать GetStandardFunctionName с локальным именем функции
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Отобразить результат
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Использовать стандартную функцию в формуле ячейки
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Вычислить формулу
                workbook.CalculateFormula();

                // Отобразить результат
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


