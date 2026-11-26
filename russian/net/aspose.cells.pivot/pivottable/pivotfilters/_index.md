---
title: "PivotTable.PivotFilters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает все фильтры в сводной таблице"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Возвращает все фильтры в сводной таблице.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Создайте сводную таблицу
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Добавьте поля в сводную таблицу
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Получить доступ к коллекции PivotFilters (свойство только для чтения)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Отобразить информацию о коллекции PivotFilters
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Итерировать фильтры и отобразить их типы
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Добавить пример фильтра для демонстрации функциональности
                if (pivotFilters.Count == 0)
                {
                    // Добавить фильтр по значению к первому полю (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Отобразить обновлённое количество фильтров
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Сохраните книгу
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


