---
title: "AdvancedFilter.CriteriaRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AdvancedFilter. Obtiene el rango de criterios de este filtro avanzado"
type: docs
url: /es/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Obtiene el rango de criterios de este filtro avanzado.

```csharp
public string CriteriaRange { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para el rango de lista
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Poblar criterios de ejemplo (el filtro usará esto cuando se aplique)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Obtener el objeto AdvancedFilter para la hoja de cálculo
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // Las propiedades ListRange, CriteriaRange y CopyToRange son de solo lectura.
                // Mostrar los rangos determinados automáticamente.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Guardar el libro de trabajo (opcional, solo para mostrar que el archivo puede ser creado)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


