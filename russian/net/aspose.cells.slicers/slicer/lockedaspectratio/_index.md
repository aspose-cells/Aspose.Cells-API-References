---
title: "Slicer.LockedAspectRatio"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Указывает, включена ли блокировка соотношения сторон"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/lockedaspectratio/
---
## Slicer.LockedAspectRatio property

Указывает, включена ли блокировка соотношения сторон.

```csharp
[Obsolete("Use Shape.IsLockAspectRatio property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LockedAspectRatio { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод [`IsAspectRatioLocked`](../../../aspose.cells.drawing/shape/isaspectratiolocked/). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(30);

            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "GroceryTable";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "A5");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.LockedAspectRatio = true;

            workbook.Save("SlicerLockedAspectRatioDemo.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


