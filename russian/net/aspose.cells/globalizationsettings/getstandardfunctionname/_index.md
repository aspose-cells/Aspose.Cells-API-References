---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает стандартное имя функции в соответствии с заданным зависимым от локали именем функции"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Получает стандартное название функции в соответствии с заданным названием функции, зависящим от локали.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Подготовить примерные данные
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Создать пользовательские настройки глобализации и назначить их рабочей книге
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Продемонстрировать GetStandardFunctionName с немецким именем функции SUM
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Применить локализованное имя функции в формуле
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Преобразовать немецкое имя функции в стандартный английский
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


