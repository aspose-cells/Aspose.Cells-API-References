---
title: "SmartTagProperty.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagProperty. Obtiene y establece el nombre de la propiedad"
type: docs
url: /es/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Obtiene y establece el nombre de la propiedad.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una instancia de SmartTagProperty usando reflexión ya que el constructor no es público
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Establezca la propiedad Name
                property.Name = "Department";

                // Mostrar el valor actual de la propiedad Name
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Demuestra cómo cambiar la propiedad Name
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Muestra que la propiedad puede leerse y modificarse
                Console.WriteLine("Name property demonstration completed successfully");
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


