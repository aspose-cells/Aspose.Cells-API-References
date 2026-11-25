---
title: "Slicer.IsLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Indica se la forma dello slicer è bloccata"
type: docs
url: /it/net/aspose.cells.slicers/slicer/islocked/
---
## Slicer.IsLocked property

Indica se la forma dello slicer è bloccata.

```csharp
[Obsolete("Use Shape.IsLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLocked { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`IsLocked`](../../../aspose.cells.drawing/shape/islocked/). Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


