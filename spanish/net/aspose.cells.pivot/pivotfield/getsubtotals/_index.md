---
title: "PivotField.GetSubtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Indica si se debe mostrar el subtotal especificado para este campo pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Indica si se muestra el subtotal especificado para este campo de tabla dinámica.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Tipo de subtotal. |

### Valor de retorno

Devuelve si se está mostrando el subtotal especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Verificar si el subtotal Sum está habilitado
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Verificar si el subtotal Average está habilitado
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Habilitar subtotal Sum
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Verificar que el subtotal Sum ahora está habilitado
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Actualiza la tabla dinámica para mostrar los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


