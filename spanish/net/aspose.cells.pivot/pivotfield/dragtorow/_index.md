---
title: "PivotField.DragToRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotField. Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToRow { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToRow. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Quarter";
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q3";
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;

            // Crear tabla dinámica y obtener su índice.
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenga el campo de fila y establezca la propiedad DragToRow
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToRow = true; // This allows the field to be dragged to row area

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldDragToRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


