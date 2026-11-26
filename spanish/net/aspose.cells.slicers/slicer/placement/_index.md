---
title: "Slicer.Placement"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo."
type: docs
url: /es/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad [`Placement`](../../../aspose.cells.drawing/shape/placement/). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
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
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar un slicer para la tabla dinámica
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Establecer propiedades del slicer incluyendo Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Guarda el libro de trabajo
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


