---
title: "Slicer.AlternativeText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve o establece la cadena de texto alternativa descriptiva del objeto Slicer"
type: docs
url: /es/net/aspose.cells.slicers/slicer/alternativetext/
---
## Slicer.AlternativeText property

Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer.

```csharp
[Obsolete("Use Shape.AlternativeText property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AlternativeText { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [`AlternativeText`](../../../aspose.cells.drawing/shape/alternativetext/). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1:A3", "", true)];
            table.DisplayName = "Table1";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "C1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.AlternativeText = "AlternativeText test";

            workbook.Save("SlicerAlternativeTextDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


