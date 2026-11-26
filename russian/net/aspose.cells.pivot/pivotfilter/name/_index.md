---
title: "PivotFilter.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Получает имя сводного фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Получает имя сводного фильтра.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить лист образцовыми данными
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;

            // Добавить сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить и настроить сводный фильтр
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Name = "ProductFilter"; // Demonstrating Name property usage
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Обновить и вычислить данные сводной таблицы
            pivot.RefreshData();
            pivot.CalculateData();

            // Сохраните книгу
            book.Save("PivotFilterNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


