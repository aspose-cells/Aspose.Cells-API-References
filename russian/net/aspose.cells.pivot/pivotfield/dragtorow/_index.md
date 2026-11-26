---
title: "PivotField.DragToRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, может ли указанное поле быть перетащено в область строк. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Указывает, может ли указанный поле быть перетянуто в область строк. Значение по умолчанию — true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToRow { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToRow. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Quarter";
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q3";
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;

            // Создайте сводную таблицу и получите её индекс.
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получите поле строки и установите свойство DragToRow
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToRow = true; // This allows the field to be dragged to row area

            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldDragToRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


