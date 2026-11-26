---
title: "PivotField.DragToColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, может ли указанное поле быть перетянуто в область столбцов. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Указывает, может ли указанный поле быть перетянуто в область столбцов. Значение по умолчанию — true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToColumn property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToColumn { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToColumn. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToColumnDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Item");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(8);

            // Добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получите поле данных и установите DragToColumn в true.
            PivotField quantityField = pivotTable.DataFields[0];
            quantityField.DragToColumn = true; // This allows the field to be dragged to column area
            quantityField.DisplayName = "Total Quantity";

            // Вычислите данные и сохраните
            pivotTable.CalculateData();
            workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


