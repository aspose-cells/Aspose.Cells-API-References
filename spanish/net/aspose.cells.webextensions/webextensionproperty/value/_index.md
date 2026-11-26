---
title: "WebExtensionProperty.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionProperty. Obtiene y establece un valor de propiedad personalizado"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Obtiene y establece un valor de propiedad personalizada.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Establecer y demostrar la propiedad Value
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Modificar y mostrar el valor actualizado
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


