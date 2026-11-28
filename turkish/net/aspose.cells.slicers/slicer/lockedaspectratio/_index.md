---
title: "Slicer.LockedAspectRatio"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer özelliği. En‑boy oranının kilitlenip kilitlenmediğini belirtir"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/lockedaspectratio/
---
## Slicer.LockedAspectRatio property

En‑boy oranının kilitlenip kilitlenmediğini belirtir.

```csharp
[Obsolete("Use Shape.IsLockAspectRatio property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LockedAspectRatio { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`IsAspectRatioLocked`](../../../aspose.cells.drawing/shape/isaspectratiolocked/) yöntemini kullanın. Bu özellik Ocak 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

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

### Ayrıca Bakınız

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


