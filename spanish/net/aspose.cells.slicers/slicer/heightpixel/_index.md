---
title: "Slicer.HeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve o establece la altura del slicer especificado en píxeles"
type: docs
url: /es/net/aspose.cells.slicers/slicer/heightpixel/
---
## Slicer.HeightPixel property

Devuelve o establece la altura del slicer especificado, en píxeles.

```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Height. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";

            int tableIndex = worksheet.ListObjects.Add("A1", "A4", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            int slicerIndex = worksheet.Slicers.Add(table, 0, "D1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.HeightPixel = 150;

            workbook.Save("SlicerHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


