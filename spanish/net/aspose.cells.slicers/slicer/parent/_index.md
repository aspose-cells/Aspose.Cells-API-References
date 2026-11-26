---
title: "Slicer.Parent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve el objeto Worksheet que contiene este segmentador. Solo lectura"
type: docs
url: /es/net/aspose.cells.slicers/slicer/parent/
---
## Slicer.Parent property

Devuelve el objeto [`Worksheet`](../worksheet/) que contiene este segmentador. Solo lectura.

```csharp
[Obsolete("Use Slicer.Worksheet property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Worksheet Parent { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [`Worksheet`](../worksheet/). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyParentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";

            int tableIndex = sheet.ListObjects.Add("A1", "A4", true);
            ListObject table = sheet.ListObjects[tableIndex];

            int slicerIndex = sheet.Slicers.Add(table, 0, "B1");
            Slicer slicer = sheet.Slicers[slicerIndex];
            Worksheet currSheet = slicer.Parent;

            currSheet.Cells["C1"].Value = "ParentWorksheetAccessed";
            workbook.Save("SlicerParentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


