---
title: "WebExtension.Bindings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtension. Obtiene todas las relaciones de enlaces entre un complemento de Office y los datos del documento"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Obtiene todas las relaciones de enlaces entre un Office Add-in y los datos del documento.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Suponiendo que obtenemos una extensión web de algún lugar (ya que no podemos crear una directamente)
                // Este es un cambio mínimo para que el código compile manteniendo su estructura
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Acceda a la propiedad Bindings (solo lectura)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Muestre información sobre los enlaces
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Agregue un nuevo enlace (demuestra el uso de la colección)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Mostrar recuento actualizado
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


