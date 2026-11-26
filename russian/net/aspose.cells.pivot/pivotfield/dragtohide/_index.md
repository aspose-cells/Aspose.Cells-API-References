---
title: "PivotField.DragToHide"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, может ли это поле сводной таблицы быть удалено из представления PivotTable. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/dragtohide/
---
## PivotField.DragToHide property

Указывает, может ли данное поле сводки быть удалено из представления сводной таблицы. Значение по умолчанию — true.

```csharp
[Obsolete("Use PivotField.AllowRemovingFromView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToHide { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.AllowRemovingFromView. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToHideDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;
            cells["B5"].Value = 250;

            // Создать сводную таблицу — сначала получить индекс, затем объект PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки и настроить DragToHide
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToHide = true; // Core demonstration of the property
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Обновить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldDragToHideDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


