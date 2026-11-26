---
title: "Clase AdvancedFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AdvancedFilter. Representa la configuración del filtro avanzado"
type: docs
url: /es/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Representa la configuración del filtro avanzado.

```csharp
public class AdvancedFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Obtiene el rango donde se copia el resultado de este filtro avanzado. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Obtiene el rango de criterios de este filtro avanzado. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Obtiene el rango de lista de este filtro avanzado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Poblar datos de ejemplo para el rango de lista
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Poblar rango de criterios
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Obtener la instancia AdvancedFilter de la hoja de cálculo
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Mostrar las propiedades de solo lectura
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Guarda el libro de trabajo
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


