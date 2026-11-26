---
title: "PivotAreaFilter.SetSubtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotAreaFilter. Subtotal para el filtro"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafilter/setsubtotals/
---
## PivotAreaFilter.SetSubtotals method

Subtotal para el filtro.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | La función de subtotal. |
| mostrado | Booleano | Indica si se muestra esta información de subtotal. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 8;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crear un área de tabla dinámica con el parámetro de tabla dinámica
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = new PivotAreaFilter();

            try
            {
                // Llamar a SetSubtotals con el tipo de subtotal Sum y configurarlo para mostrar
                filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                
                // Verificar si el subtotal está configurado
                bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is set: {isSumSet}");

                // Actualizar la tabla dinámica para ver los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


