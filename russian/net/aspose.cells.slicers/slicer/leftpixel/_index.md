---
title: "Slicer.LeftPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Slicer property. Возвращает или задает горизонтальное смещение формы среза от её левой колонки в пикселях"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/leftpixel/
---
## Slicer.LeftPixel property

Возвращает или задает горизонтальное смещение формы среза от её левой колонки в пикселях.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Shape.Left. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLeftPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);

            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            int slicerIndex = sheet.Slicers.Add(pivotTable, "A10", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            slicer.LeftPixel = 2;

            workbook.Save("SlicerPropertyLeftPixelDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


