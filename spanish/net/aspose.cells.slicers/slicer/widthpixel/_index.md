---
title: "Slicer.WidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve o establece el ancho del slicer especificado en píxeles"
type: docs
url: /es/net/aspose.cells.slicers/slicer/widthpixel/
---
## Slicer.WidthPixel property

Devuelve o establece el ancho del slicer especificado, en píxeles.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Width. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(150);
            sheet.Cells["B3"].PutValue(200);
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            
            int slicerIndex = sheet.Slicers.Add(table, 0, "A5");
            Slicer slicer = sheet.Slicers[slicerIndex];
            slicer.LeftPixel = 50;
            slicer.TopPixel = 100;
            slicer.WidthPixel = 120;
            
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


