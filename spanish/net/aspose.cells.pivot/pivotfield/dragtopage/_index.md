---
title: "PivotField.DragToPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### Observaciones

NOTA: Esta propiedad ahora está obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToPage. Este método será eliminado 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos y configurar DragToPage
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // Demostrar la propiedad DragToPage
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guardar el libro de trabajo
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


