---
title: "Range.ClearHyperlinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Solo elimina hipervínculos"
type: docs
url: /es/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Solo elimina hipervínculos.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clearFormat | Booleano | Indica si se debe eliminar el formato de los hipervínculos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango y agregar algunos hipervínculos para demostración
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Borrar hipervínculos con preservación de formato (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Agregar hipervínculos nuevamente
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Borrar hipervínculos sin preservación de formato (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Guarda el libro de trabajo
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


