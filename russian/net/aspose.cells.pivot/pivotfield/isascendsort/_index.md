---
title: "PivotField.IsAscendSort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Указывает, автоматически ли сортируются элементы этого поля сводной таблицы по возрастанию.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendSort { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.SortSetting.SortType или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendSortDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "B";
            sheet.Cells["A3"].Value = "C";
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B2"].Value = 150;
            sheet.Cells["B3"].Value = 300;
            sheet.Cells["B4"].Value = 200;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Настройте сортировку
            PivotField sortField = pivotTable.RowFields[0];
            sortField.IsAutoSort = true;
            sortField.IsAscendSort = false; // Demonstrate descending sort
            sortField.AutoSortField = 0; // Sort by first data field
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldIsAscendSortDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


