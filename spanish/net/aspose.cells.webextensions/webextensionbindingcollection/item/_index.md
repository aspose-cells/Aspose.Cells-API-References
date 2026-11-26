---
title: "WebExtensionBindingCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionBindingCollection. Obtiene la relación de enlace de la extensión web por el índice específico"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Obtiene la relación de enlace de extensión web por el índice específico.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La relación de enlace de la extensión web

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de enlaces de extensiones web
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Agregar un nuevo enlace a la colección
            int index = bindingCollection.Add();

            // Acceder al enlace usando la propiedad Item (solo lectura)
            WebExtensionBinding binding = bindingCollection[index];

            // Establecer propiedades en el enlace
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Mostrar los detalles del enlace
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Modificar el enlace a través de la colección
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Guarda el libro de trabajo
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


