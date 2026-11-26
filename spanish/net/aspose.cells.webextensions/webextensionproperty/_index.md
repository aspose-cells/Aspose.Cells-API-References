---
title: "Clase WebExtensionProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionProperty. Representa una propiedad personalizada del complemento de Office"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Representa una propiedad personalizada de un complemento de Office.

```csharp
public class WebExtensionProperty
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Obtiene y establece un nombre de propiedad personalizada. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Obtiene y establece un valor de propiedad personalizada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Cree una nueva instancia de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Establezca valores de propiedad
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Muestra los valores de la propiedad
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


