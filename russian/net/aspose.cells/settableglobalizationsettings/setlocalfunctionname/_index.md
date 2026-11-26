---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает зависящее от локали имя функции, соответствующее заданному стандартному имени функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Устанавливает зависящее от локали имя функции, соответствующее заданному стандартному имени функции.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | String | Стандартное имя функции (локаль en-US). |
| localName | String | Зависящее от локали имя функции |
| bidirectional | Boolean | Определяет, следует ли автоматически сопоставлять локальное имя функции со стандартным именем функции. Если true, локальное имя будет автоматически сопоставлено со стандартным именем, поэтому пользователю не нужно снова вызывать [`SetStandardFunctionName`](../setstandardfunctionname/) для той же пары стандартного и локального имен. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Вызвать SetLocalFunctionName для сопоставления стандартного имени функции с локальным именем
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Создать формулы, использующие как стандартные, так и локализованные имена
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Вычислить формулы
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


