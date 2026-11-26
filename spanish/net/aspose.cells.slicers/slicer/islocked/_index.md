---
title: "Slicer.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Indica si la forma del slicer está bloqueada"
type: docs
url: /es/net/aspose.cells.slicers/slicer/islocked/
---
## Slicer.IsLocked property

Indica si la forma del slicer está bloqueada.

```csharp
[Obsolete("Use Shape.IsLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLocked { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad [`IsLocked`](../../../aspose.cells.drawing/shape/islocked/). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

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

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


