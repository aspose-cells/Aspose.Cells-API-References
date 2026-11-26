---
title: "WebExtensionBinding.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionBinding. Obtiene y establece el identificador del enlace"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Obtiene y establece el identificador de enlace.

```csharp
public string Id { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyIdDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva instancia de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Establecer la propiedad Id
                binding.Id = "SampleBindingId";
                
                // Mostrar el valor actual de Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Modificar el valor de Id para demostrar que es de lectura/escritura
                binding.Id = "UpdatedBindingId";
                Console.WriteLine("Updated Id value: " + binding.Id);
                
                Console.WriteLine("Id property has been successfully demonstrated");
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

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


