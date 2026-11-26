---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает название функции, зависящее от локали, в соответствии с заданным стандартным названием функции"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Получает название функции, зависящее от локали, в соответствии с заданным стандартным названием функции.

```csharp
public virtual string GetLocalFunctionName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить пользовательские настройки глобализации
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Добавьте примерные данные
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Создать формулу с локализованным названием функции
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


