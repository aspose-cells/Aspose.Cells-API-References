---
title: "GlobalizationSettings.Compare"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Сравнивает две строковые величины согласно определённым правилам сортировки"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

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

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу с пользовательскими настройками глобализации
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Продемонстрировать прямое использование метода Compare
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Продемонстрировать влияние на операции с электронными таблицами
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Сортировать данные с использованием пользовательского сравнения
                DataSorter sorter = workbook.DataSorter;
                sorter.Order1 = SortOrder.Ascending;
                sorter.Key1 = 0;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2

                Console.WriteLine("Sorted data with custom comparison rules:");
                for (int row = 0; row < 3; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }

                workbook.Save("GlobalizationCompareDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomComparisonSettings : GlobalizationSettings
    {
        public override int Compare(string v1, string v2, bool ignoreCase)
        {
            // Реализовать логику пользовательского сравнения
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


