---
title: "PivotFilter.AutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Получает автофильтр сводного фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

Получает автофильтр сводного фильтра.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте методы FilterLabel, FilterValue, FilterDate или FilterTop10. Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавьте лист и заполните его образцовыми данными
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Добавить фильтр в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.PageFields[0];

            // Создать и добавить фильтр
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];

            try
            {
                // Отобразить значение свойства AutoFilter (только для чтения)
                Console.WriteLine("AutoFilter Range: " + filter.AutoFilter.Range);
                Console.WriteLine("AutoFilter ShowFilterButton: " + filter.AutoFilter.ShowFilterButton);

                // Продемонстрировать доступ к свойствам AutoFilter
                Console.WriteLine("AutoFilter has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("PivotFilterAutoFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


