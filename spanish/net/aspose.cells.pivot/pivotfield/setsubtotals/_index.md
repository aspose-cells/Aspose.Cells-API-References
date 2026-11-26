---
title: "PivotField.SetSubtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Establece cómo subtotalizar el campo especificado."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Establece cómo subtotalizar el campo especificado.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| mostrado | Booleano | Indica si el campo especificado muestra subtotales. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // Agregar tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Agregar campos de fila
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Demostrar SetSubtotals con PivotFieldSubtotalType y booleano.
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


