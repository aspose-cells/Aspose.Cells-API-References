---
title: "WebExtensionBinding.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionBinding. Obtiene y establece el tipo de enlace"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Obtiene y establece el tipo de enlace.

```csharp
public string Type { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva instancia de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Establecer la propiedad Type
                binding.Type = "text";
                
                // Mostrar el valor actual de Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Modificar el valor de Type para demostrar que es de lectura/escritura
                binding.Type = "range";
                Console.WriteLine("Updated Type value: " + binding.Type);
                
                Console.WriteLine("Type property has been successfully demonstrated");
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


