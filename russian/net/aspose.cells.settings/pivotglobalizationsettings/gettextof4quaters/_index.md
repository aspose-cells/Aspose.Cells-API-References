---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotGlobalizationSettings. Получает локальный текст 4 кварталов"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Получает локальный текст 4 кварталов.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetTextOf4Quarters(). Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательский класс настроек глобализации, наследующий от PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Вызовите метод GetTextOf4Quaters
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Выведите названия кварталов в консоль
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Добавьте названия кварталов в лист
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Пользовательская реализация PivotGlobalizationSettings для переопределения GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Возвратить пользовательские названия кварталов
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### См. также

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


