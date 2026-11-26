---
title: "PivotFilterCollection.ClearFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Очистить PivotFilter из конкретного PivotField"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/clearfilter/
---
## PivotFilterCollection.ClearFilter method

Очистить PivotFilter из конкретного PivotField

```csharp
public void ClearFilter(int fieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | индекс PivotField |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodClearFilterWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить фильтр к сводной таблице
            PivotFilterCollection filters = pivotTable.PivotFilters;
            filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);

            try
            {
                // Вызвать метод ClearFilter с параметром индекса поля
                filters.ClearFilter(0);
                
                Console.WriteLine("Pivot filter cleared successfully for field index 0");
                
                // Проверить, что фильтр был очищен
                Console.WriteLine($"Number of filters after clearing: {filters.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


