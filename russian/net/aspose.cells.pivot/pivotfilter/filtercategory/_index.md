---
title: "PivotFilter.FilterCategory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Получает категорию этого фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/filtercategory/
---
## PivotFilter.FilterCategory property

Получает категорию этого фильтра.

```csharp
public FilterCategory FilterCategory { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyFilterCategoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать пример данных сводной таблицы
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                worksheet.Cells["B1"].Value = "Value";
                worksheet.Cells["B2"].Value = 100;
                worksheet.Cells["B3"].Value = 200;
                worksheet.Cells["B4"].Value = 300;

                // Создать сводную таблицу
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Добавить поле строки, используя правильный метод API
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                
                // Добавить поле данных, используя правильный метод API
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;
                dataField.DisplayName = "Total";

                // Добавить фильтр заголовка к полю Category
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Отобразить значение свойства FilterCategory
                Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);

                workbook.Save("FilterCategoryDemo.xlsx");
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

* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


