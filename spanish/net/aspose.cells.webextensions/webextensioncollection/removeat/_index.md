---
title: "WebExtensionCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebExtensionCollection. Elimina la extensión web por el índice"
type: docs
url: /es/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Eliminar la extensión web por el índice.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear colección de extensiones web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Agregar algunas extensiones web a la colección
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Llame al método RemoveAt con el parámetro Int32
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


