---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | String | Зависящее от локали имя функции |
| standardName | String | Стандартное имя функции (локаль en-US). |
| bidirectional | Boolean | Определяет, следует ли автоматически сопоставлять стандартное имя функции с локальным именем функции. Если true, стандартное имя будет автоматически сопоставлено с локальным, и пользователю не понадобится вызывать [`SetLocalFunctionName`](../setlocalfunctionname/) снова для той же пары стандартных и локальных имен. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Вызовите SetStandardFunctionName, чтобы сопоставить локальное имя функции со стандартным именем
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Создайте формулу, используя локальное имя функции
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Вычислить формулу
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


