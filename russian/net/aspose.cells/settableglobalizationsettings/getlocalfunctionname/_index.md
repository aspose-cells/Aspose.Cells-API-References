---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает зависящее от локали имя функции в соответствии с заданным стандартным именем функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Получает название функции, зависящее от локали, в соответствии с заданным стандартным названием функции.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | String | Стандартное имя функции (локаль en-US). |

### Возвращаемое значение

Имя функции, зависящее от локали. Локаль была указана в Workbook, для которого используются эти настройки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установите пользовательское локальное имя функции для "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызовите GetLocalFunctionName, чтобы получить локализованное имя
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Отобразить результат
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Используйте локализованную функцию в ячейке
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Вычислить формулы
                workbook.CalculateFormula();

                // Отобразить результат
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


