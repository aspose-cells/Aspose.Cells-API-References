---
title: Slicer.LockedAspectRatio
second_title: Aspose.Cells for .NET API Reference
description: Slicer property. Indicates whether locking aspect ratio
type: docs
url: /net/aspose.cells.slicers/slicer/lockedaspectratio/
---
## Slicer.LockedAspectRatio property

Indicates whether locking aspect ratio.

```csharp
[Obsolete("Use Shape.GetLockedProperty() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LockedAspectRatio { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use !:Shape.GetLockedProperty() method. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

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

### See Also

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


