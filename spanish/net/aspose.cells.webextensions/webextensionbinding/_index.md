---
title: "Clase WebExtensionBinding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionBinding. Representa una relación de enlace entre un complemento de Office y los datos del documento"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Representa una relación de enlace entre un complemento de Office y los datos del documento.

```csharp
public class WebExtensionBinding
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Obtiene y establece la clave de enlace utilizada para mapear la entrada de enlace en esta lista con los datos vinculados en el documento. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Obtiene y establece el identificador de enlace. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Obtiene y establece el tipo de enlace. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva instancia de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();

                // Establecer propiedades
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Mostrar valores de propiedades
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Modificar propiedades
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


