---
title: "PivotField.DragToData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToData. Este método será eliminado 12 meses después desde julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila y configurar DragToData
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Agregar campo de columna
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


