---
title: "PivotFilter.AutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el autofiltro del filtro pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

Obtiene el autofiltro del filtro pivote.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice los métodos FilterLabel, FilterValue,FilterDate o FilterTop10. Este método será eliminado 12 meses después, desde noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Agregar un filtro a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.PageFields[0];

            // Crear y agregar filtro
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];

            try
            {
                // Mostrar el valor de la propiedad AutoFilter (solo lectura)
                Console.WriteLine("AutoFilter Range: " + filter.AutoFilter.Range);
                Console.WriteLine("AutoFilter ShowFilterButton: " + filter.AutoFilter.ShowFilterButton);

                // Demostrar el acceso a las propiedades AutoFilter
                Console.WriteLine("AutoFilter has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotFilterAutoFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


