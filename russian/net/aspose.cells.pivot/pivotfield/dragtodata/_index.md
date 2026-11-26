---
title: "PivotField.DragToData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Указывает, может ли указанный поле быть перетянуто в область значений. Значение по умолчанию — true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToData. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавьте поле строки и настройте DragToData
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Добавить поле столбца
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


