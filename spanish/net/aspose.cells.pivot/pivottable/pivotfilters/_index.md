---
title: "PivotTable.PivotFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve todos los filtros en la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Devuelve todos los filtros en la tabla dinámica.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Crear una tabla dinámica
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Agregar campos a la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Acceder a la colección PivotFilters (propiedad de solo lectura)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Mostrar información sobre la colección PivotFilters
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Iterar a través de los filtros y mostrar sus tipos
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Agregar un filtro de ejemplo para demostrar la funcionalidad
                if (pivotFilters.Count == 0)
                {
                    // Agregar un filtro de valor al primer campo (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Mostrar el recuento actualizado de filtros
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Guarda el libro de trabajo
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


