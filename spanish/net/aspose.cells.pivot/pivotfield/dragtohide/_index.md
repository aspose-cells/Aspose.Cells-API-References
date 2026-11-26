---
title: "PivotField.DragToHide"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si este campo dinámico puede ser eliminado de la vista de la PivotTable. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/dragtohide/
---
## PivotField.DragToHide property

Indica si este campo de tabla dinámica puede eliminarse de la vista de la tabla dinámica. El valor predeterminado es true.

```csharp
[Obsolete("Use PivotField.AllowRemovingFromView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToHide { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowRemovingFromView. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToHideDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;
            cells["B5"].Value = 250;

            // Crear tabla dinámica - Obtenga primero el índice, luego obtenga el objeto PivotTable.
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila y configurar DragToHide
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToHide = true; // Core demonstration of the property
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldDragToHideDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


