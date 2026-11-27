---
title: "Slicer.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer property. Anger om slicerformen är låst"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/islocked/
---
## Slicer.IsLocked property

Anger om slicerformen är låst.

```csharp
[Obsolete("Use Shape.IsLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLocked { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället [`IsLocked`](../../../aspose.cells.drawing/shape/islocked/) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


