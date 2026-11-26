---
title: "Clase CustomFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CustomFilter. Representa el filtro personalizado"
type: docs
url: /es/net/aspose.cells/customfilter/
---
## CustomFilter class

Representa el filtro personalizado.

```csharp
public class CustomFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Obtiene y establece los criterios. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Obtiene y establece el tipo de operador del filtro. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Establece los criterios del filtro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Aplicar filtro automático al rango
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Aplicar un filtro personalizado para obtener una instancia de CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Obtener el primer filtro personalizado de la colección de filtros
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Mostrar las propiedades del filtro
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Modificar los criterios del filtro usando el método SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Mostrar las propiedades del filtro actualizadas
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Guarda el libro de trabajo
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


