---
title: "SmartTagProperty.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagProperty. Obtiene y establece el valor de la propiedad"
type: docs
url: /es/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Obtiene y establece el valor de la propiedad.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una instancia de SmartTagProperty usando el constructor no público
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Establece el nombre y el valor de la propiedad
                property.Name = "Category";
                property.Value = "Finance";

                // Muestra los valores de la propiedad
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
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

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


