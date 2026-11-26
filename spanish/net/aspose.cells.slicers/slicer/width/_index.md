---
title: "Slicer.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Slicer. Devuelve o establece el ancho del slicer especificado en puntos."
type: docs
url: /es/net/aspose.cells.slicers/slicer/width/
---
## Slicer.Width property

Devuelve o establece el ancho del slicer especificado, en puntos.

```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.WidthPt. Esta propiedad será eliminada 12 meses después, a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar un segmentador
            int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Forma correcta de agregar la conexión de tabla dinámica al slicer.
            slicer.AddPivotConnection(pivotTable);

            // Establecer propiedades del slicer, incluyendo el ancho.
            slicer.Caption = "Fruit Selection";
            slicer.Width = 150; // Setting the width in points
            slicer.Height = 200;

            // Guarda el libro de trabajo
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


