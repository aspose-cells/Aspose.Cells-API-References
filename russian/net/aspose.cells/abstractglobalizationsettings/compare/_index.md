---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractGlobalizationSettings. Сравнивает два строковых значения согласно определённым правилам сортировки"
type: docs
url: /ru/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

Сравнивает два строковых значения в соответствии с определёнными правилами сортировки.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| v1 | String | первая строка |
| v2 | String | вторая строка |
| ignoreCase | Boolean | нужно ли игнорировать регистр при сравнении значений |

### Возвращаемое значение

Целое число, указывающее лексическое отношение между двумя сравниваемыми

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать пользовательские настройки глобализации, переопределяющие метод Compare
            var settings = new CustomGlobalizationSettings();
            
            // Создать книгу с пользовательскими настройками глобализации
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Подготовить строки для сравнения
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // Метод Compare будет вызываться внутри во время операций, таких как сортировка
                // Здесь мы демонстрируем прямое использование
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Продемонстрировать эффект, сортируя данные
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Создать DataSorter и задать диапазон для сортировки
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### См. также

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


