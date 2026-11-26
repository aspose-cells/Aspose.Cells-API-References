---
title: "Range.ClearComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Elimina los comentarios de este rango"
type: docs
url: /es/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Borra los comentarios de este rango.

```csharp
public void ClearComments()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos y comentarios a las celdas
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Crear un rango que incluya celdas con comentarios
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Eliminar comentarios del rango
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Guarda el libro de trabajo
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


