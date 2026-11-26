---
title: "AdvancedFilter.CopyToRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AdvancedFilter. Obtiene el rango al que se copia el resultado de este filtro avanzado"
type: docs
url: /es/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Obtiene el rango donde se copia el resultado de este filtro avanzado.

```csharp
public string CopyToRange { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Agregar rango de criterios
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Obtener la instancia AdvancedFilter de la hoja de cálculo
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Mostrar el valor de la propiedad CopyToRange
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Guarda el libro de trabajo
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


