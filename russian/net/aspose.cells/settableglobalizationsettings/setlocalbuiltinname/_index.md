---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает зависящий от локали текст для встроенного имени с заданным текстом стандартного имени"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Устанавливает зависящий от локали текст для встроенного имени с заданным стандартным текстом имени.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | String | Текст стандартного (en-US) имени встроенного названия. |
| localName | String | Текст имени, зависящий от локали |
| bidirectional | Boolean | Определяет, следует ли автоматически сопоставлять текст локального имени со стандартным текстом имени. Если true, текст локального имени будет автоматически сопоставлен со стандартным, и пользователю не понадобится вызывать [`SetStandardBuiltInName`](../setstandardbuiltinname/) снова для той же пары стандартных и локальных имен. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // Вызовите SetLocalBuiltInName, чтобы сопоставить стандартное встроенное имя с локальным именем
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Создайте формулу, используя стандартное встроенное имя
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Вычислить формулу
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Проверьте сопоставление локального имени
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


