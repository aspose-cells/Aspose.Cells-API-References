---
title: "PivotField.IsAutoSubtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es true."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSubtotalsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo al área de filas y establecer IsAutoSubtotals en false
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.IsAutoSubtotals = false; // Disable automatic subtotals

            // Agregar campo al área de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcular datos
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


