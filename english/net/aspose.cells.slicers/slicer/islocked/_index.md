---
title: Slicer.IsLocked
second_title: Aspose.Cells for .NET API Reference
description: Slicer property. Indicates whether the slicer shape is locked
type: docs
url: /net/aspose.cells.slicers/slicer/islocked/
---
## Slicer.IsLocked property

Indicates whether the slicer shape is locked.

```csharp
[Obsolete("Use Shape.IsLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLocked { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use [`IsLocked`](../../../aspose.cells.drawing/shape/islocked/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];
            
            int slicerIndex = worksheet.Slicers.Add(table, 0, "D1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.IsLocked = false;

            worksheet.Protect(ProtectionType.All, "password", null);
            workbook.Save("SlicerIsLockedDemo.xlsx");
        }
    }
}
```

### See Also

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


