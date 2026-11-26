---
title: "PivotField.DragToColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es true."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToColumn property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToColumn { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToColumn. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToColumnDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Item");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(8);

            // Agregar una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtenga el campo de datos y establezca DragToColumn en true.
            PivotField quantityField = pivotTable.DataFields[0];
            quantityField.DragToColumn = true; // This allows the field to be dragged to column area
            quantityField.DisplayName = "Total Quantity";

            // Calcular datos y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


