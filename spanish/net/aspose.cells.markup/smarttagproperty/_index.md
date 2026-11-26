---
title: "Clase SmartTagProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Markup.SmartTagProperty. Representa la propiedad de la etiqueta inteligente de la celda"
type: docs
url: /es/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Representa la propiedad de la etiqueta inteligente de la celda.

```csharp
public class SmartTagProperty
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Obtiene y establece el nombre de la propiedad. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Obtiene y establece el valor de la propiedad. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una instancia de SmartTagProperty usando reflexión ya que el constructor no es público
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Establece las propiedades Name y Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Muestra los valores de la propiedad
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Demuestra la modificación de las propiedades
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


