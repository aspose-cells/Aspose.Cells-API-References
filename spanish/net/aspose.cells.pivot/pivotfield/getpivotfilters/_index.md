---
title: "PivotField.GetPivotFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Obtiene los filtros pivot del pivot field"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getpivotfilters/
---
## PivotField.GetPivotFilters method

Obtiene los filtros pivot del pivot field

```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.GetFilters(). Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotFieldMethodGetPivotFiltersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos de tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Llame al método GetPivotFilters (obsoleto)
                ArrayList pivotFilters = pivotField.GetPivotFilters();
                
                Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
                
                // Alternativamente, use el método GetFilters() no obsoleto
                PivotFilter[] filters = pivotField.GetFilters();
                Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodGetPivotFiltersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


