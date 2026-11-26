---
title: "WebExtensionBinding.Appref"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionBinding. Obtiene y establece la clave de enlace utilizada para mapear la entrada de enlace en esta lista con los datos vinculados en el documento"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Obtiene y establece la clave de enlace utilizada para mapear la entrada de enlace en esta lista con los datos vinculados en el documento.

```csharp
public string Appref { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyApprefDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva instancia de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Establecer propiedades, incluido Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Mostrar el valor actual de Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Modificar el valor de Appref para demostrar que es de lectura/escritura
                binding.Appref = "Sheet1!C3:D4";
                Console.WriteLine("Updated Appref value: " + binding.Appref);
                
                Console.WriteLine("Appref property has been successfully demonstrated");
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


