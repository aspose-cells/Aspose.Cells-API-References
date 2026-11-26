---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает стандартный текст встроенного имени в соответствии с заданным локализованным текстом"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | String | Текст встроенного имени, зависящий от локали. Локаль была указана книгой Excel, для которой используются эти настройки. |

### Возвращаемое значение

Стандартный текст (локаль en-US).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу с пользовательскими настройками глобализации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Инициализировать пользовательские настройки глобализации и назначить их книге
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Тестовый параметр для GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Вызвать GetStandardBuiltInName с локальным именем функции
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Продемонстрировать эффект, используя локальное имя в формуле
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Вычислить формулу, чтобы показать правильную интерпретацию
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Пользовательские настройки глобализации, переопределяющие GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Отобразить пользовательское локальное имя функции на стандартную SUM
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


