---
title: "CustomFilterCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomFilterCollection. Obtiene el filtro personalizado en el índice específico"
type: docs
url: /es/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Obtiene el filtro personalizado en el índice específico.

```csharp
public CustomFilter this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Crear una nueva CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Acceder a la propiedad Item (solo lectura) usando el indexador
                // Dado que la colección está vacía, solo demostraremos el acceso a la propiedad
                // En un escenario real, primero agregarías filtros por otros medios
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Guarda el libro de trabajo
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


