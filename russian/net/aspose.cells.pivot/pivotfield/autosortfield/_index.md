---
title: "PivotField.AutoSortField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Представляет индекс поля, которое автоматически сортируется. 1 означает само поле PivotField, остальные значения означают позицию полей данных."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Представляет индекс поля, которое автоматически сортируется. -1 означает само поле PivotField, остальные значения означают позицию полей данных.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.SortSetting.SortBy или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Настройте автоматическую сортировку
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Вычислить данные и обновить
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


