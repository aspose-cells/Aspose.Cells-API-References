---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает строковое значение для отображения ошибки ячейки"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Получает отображаемое строковое значение ошибки ячейки.

```csharp
public virtual string GetErrorValueString(string err)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ошибка | String | значения ошибок, такие как #VALUE!,#NAME? |

### Возвращаемое значение

По умолчанию возвращает само значение ошибки

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить пользовательские настройки глобализации
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Создать сценарий ошибки: деление на ноль
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // Пользовательские сопоставления значений ошибок
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


