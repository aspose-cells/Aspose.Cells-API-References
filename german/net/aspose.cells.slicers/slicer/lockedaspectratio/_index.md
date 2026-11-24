---
title: "Slicer.LockedAspectRatio"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt an, ob das Seitenverhältnis gesperrt wird."
type: docs
url: /de/net/aspose.cells.slicers/slicer/lockedaspectratio/
---
## Slicer.LockedAspectRatio property

Gibt an, ob das Seitenverhältnis gesperrt wird.

```csharp
[Obsolete("Use Shape.IsLockAspectRatio property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LockedAspectRatio { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [`IsAspectRatioLocked`](../../../aspose.cells.drawing/shape/isaspectratiolocked/)‑Methode. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

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

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


