---
title: "Slicer.Placement"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Slicer property. Представляет способ, которым графический объект прикреплен к ячейкам под ним. Свойство управляет размещением объекта на листе."
type: docs
url: /ru/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Представляет способ, которым объект рисунка прикреплен к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [`Placement`](../../../aspose.cells.drawing/shape/placement/). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить срез для сводной таблицы
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Установить свойства среза, включая Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Сохраните книгу
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


