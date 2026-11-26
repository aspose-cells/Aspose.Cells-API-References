---
title: "PivotField.GetPivotFilters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Получает фильтры сводной таблицы для данного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/getpivotfilters/
---
## PivotField.GetPivotFilters method

Получает фильтры сводной таблицы для данного поля

```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.GetFilters(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotFieldMethodGetPivotFiltersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поля сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Вызовите метод GetPivotFilters (устаревший)
                ArrayList pivotFilters = pivotField.GetPivotFilters();
                
                Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
                
                // В качестве альтернативы используйте неустаревший метод GetFilters()
                PivotFilter[] filters = pivotField.GetFilters();
                Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodGetPivotFiltersDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


