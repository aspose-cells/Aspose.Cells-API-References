---
title: "Slicer.TopPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Slicer. Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior en píxeles."
type: docs
url: /es/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior, en píxeles.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTopPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Crear tabla dinámica y obtener su índice.
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Agregar slicer y obtener su índice.
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Establecer la propiedad TopPixel.
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


