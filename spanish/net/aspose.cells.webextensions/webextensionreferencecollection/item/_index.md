---
title: "WebExtensionReferenceCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionReferenceCollection. Obtiene la extensión web por el índice específico"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Obtiene la extensión web por el índice específico.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La extensión web

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Agrega una nueva referencia de extensión web
                int index = references.Add();
                
                // Acceder a la propiedad Item (solo lectura) para obtener la referencia en el índice especificado
                WebExtensionReference reference = references[index];
                
                // Mostrar información sobre la referencia recuperada
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Nota: La propiedad Item es de solo lectura, por lo que solo demostramos obtener su valor
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

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


