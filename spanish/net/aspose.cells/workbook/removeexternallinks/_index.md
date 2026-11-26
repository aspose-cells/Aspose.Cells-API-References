---
title: "Workbook.RemoveExternalLinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Elimina todos los enlaces externos en el libro"
type: docs
url: /es/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Elimina todos los enlaces externos en el libro.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método ExternalLinkCollection.Clear(). Este método será eliminado 12 meses después, a partir de diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Llame al método RemoveExternalLinks
                workbook.RemoveExternalLinks();

                // Mostrar resultados o efectos de la llamada al método
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Guarde el workbook si se realizaron cambios
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


