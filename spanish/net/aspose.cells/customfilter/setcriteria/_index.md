---
title: "CustomFilter.SetCriteria"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomFilter. Establece los criterios del filtro"
type: docs
url: /es/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Establece los criterios del filtro.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filterOperator | FilterOperatorType | tipo de operador del filtro |
| criterio | Objeto | valor del criterio del filtro |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Aplicar un filtro personalizado para obtener una instancia de CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Obtener el primer filtro personalizado de la colección de filtros
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Establecer criterios usando el método SetCriteria
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Mostrar los criterios establecidos
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Guarda el libro de trabajo
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


