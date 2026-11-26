---
title: "Enumeración PivotFieldSubtotalType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. Descripción resumida para PivotFieldSubtotalType"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Descripción resumida para PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Representa el tipo de subtotal Ninguno. |
| Automatic | `1` | Representa el tipo de subtotal Automático. |
| Sum | `2` | Representa el tipo de subtotal Suma. |
| Count | `4` | Representa el tipo de subtotal Conteo. |
| Average | `8` | Representa el tipo de subtotal Promedio. |
| Max | `10` | Representa el tipo de subtotal Máximo. |
| Min | `20` | Representa el tipo de subtotal Mínimo. |
| Product | `40` | Representa el tipo de subtotal Producto. |
| CountNums | `80` | Representa el tipo de subtotal de Conteo de Números. |
| Stdev | `100` | Representa el tipo de subtotal de Desviación Estándar. |
| Stdevp | `200` | Representa el tipo de subtotal de Desviación Estándar de una Población. |
| Var | `400` | Representa el tipo de subtotal de Varianza. |
| Varp | `800` | Representa el tipo de subtotal de Varianza de una Población. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Agregar una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Establecer el tipo de subtotal para el campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


