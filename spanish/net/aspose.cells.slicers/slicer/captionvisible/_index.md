---
title: "Slicer.CaptionVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Slicer. Devuelve o establece si el encabezado que muestra el Caption del slicer es visible. El valor predeterminado es verdadero."
type: docs
url: /es/net/aspose.cells.slicers/slicer/captionvisible/
---
## Slicer.CaptionVisible property

Devuelve o establece si el encabezado que muestra el Caption del slicer es visible. El valor predeterminado es verdadero.

```csharp
[Obsolete("Use Slicer.ShowCaption property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool CaptionVisible { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [`ShowCaption`](../showcaption/). Esta propiedad será eliminada 12 meses después, a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyCaptionVisibleDemo
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
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar un segmentador
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Establecer propiedades del slicer incluyendo CaptionVisible
            slicer.Caption = "Fruit Selection";
            slicer.CaptionVisible = true; // Show the caption header
            slicer.NumberOfColumns = 2;
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Guarda el libro de trabajo
            workbook.Save("SlicerCaptionVisibleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


