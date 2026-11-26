---
title: "PivotField.IsAutoSort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, сортируются ли элементы этого поля сводной таблицы автоматически"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Указывает, сортируются ли элементы этого поля сводной таблицы автоматически.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoSort { get; set; }
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
    public class PivotFieldPropertyIsAutoSortDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Blueberry";
            cells["B5"].Value = 15;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поле строки и установить автоматическую сортировку
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsAutoSort = true;
            rowField.AutoSortField = 1; // Sort by Quantity (column B)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldIsAutoSortDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


