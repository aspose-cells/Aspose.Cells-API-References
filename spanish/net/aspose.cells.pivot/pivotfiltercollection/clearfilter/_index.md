---
title: "PivotFilterCollection.ClearFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Elimina PivotFilter del PivotField específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/clearfilter/
---
## PivotFilterCollection.ClearFilter method

Borrar PivotFilter del PivotField específico

```csharp
public void ClearFilter(int fieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | el índice del PivotField |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodClearFilterWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar filtro a la tabla dinámica
            PivotFilterCollection filters = pivotTable.PivotFilters;
            filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);

            try
            {
                // Llamar al método ClearFilter con el parámetro de índice de campo
                filters.ClearFilter(0);
                
                Console.WriteLine("Pivot filter cleared successfully for field index 0");
                
                // Verificar que el filtro fue eliminado
                Console.WriteLine($"Number of filters after clearing: {filters.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


