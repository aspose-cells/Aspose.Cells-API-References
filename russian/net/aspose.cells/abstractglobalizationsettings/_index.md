---
title: "Класс AbstractGlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AbstractGlobalizationSettings. Представляет настройки глобализации"
type: docs
url: /ru/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Представляет настройки глобализации.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Сравнивает два строковых значения в соответствии с определёнными правилами сортировки. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Создайте пользовательскую реализацию AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Продемонстрировать метод Compare
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Продемонстрировать метод GetCollationKey
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Применить настройки к рабочей книге
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Добавьте некоторые данные, чтобы продемонстрировать работу настроек
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Сохраните книгу
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


