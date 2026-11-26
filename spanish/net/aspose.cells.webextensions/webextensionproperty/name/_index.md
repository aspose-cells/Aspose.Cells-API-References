---
title: "WebExtensionProperty.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionProperty. Obtiene y establece un nombre de propiedad personalizado"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Obtiene y establece un nombre de propiedad personalizada.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Establecer y demostrar la propiedad Name
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Modificar y mostrar el nombre actualizado
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
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


