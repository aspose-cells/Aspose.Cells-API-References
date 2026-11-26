---
title: "Clase CustomProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Properties.CustomProperty. Representa una propiedad personalizada que almacena pares de nombre y valor de datos arbitrarios definidos por el usuario para la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Representa una propiedad personalizada que almacena pares de nombre y valor de datos arbitrarios definidos por el usuario para la hoja de cálculo.

```csharp
public class CustomProperty
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Obtiene y establece el valor binario de la propiedad personalizada. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Devuelve o establece el nombre del objeto. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsoleto.**) Devuelve o establece el valor de la propiedad personalizada. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Devuelve o establece el valor de la propiedad personalizada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Acceder a la colección CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Agregar propiedades personalizadas
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Acceder y mostrar las propiedades personalizadas
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


