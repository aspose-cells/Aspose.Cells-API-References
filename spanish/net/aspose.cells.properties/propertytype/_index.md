---
title: "Enum PropertyType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Properties.PropertyType. Especifica el tipo de datos de una propiedad de documento"
type: docs
url: /es/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Especifica el tipo de datos de una propiedad de documento.

```csharp
public enum PropertyType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Boolean | `0` | La propiedad es un valor booleano. |
| DateTime | `1` | La propiedad es un valor de fecha y hora. |
| Double | `2` | La propiedad es un número de punto flotante. |
| Number | `3` | La propiedad es un número entero. |
| String | `4` | La propiedad es un valor de cadena. |
| Blob | `5` | La propiedad es una matriz de bytes. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer algunas propiedades integradas
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Acceder a las propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Agregar propiedades personalizadas de diferentes tipos
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Recuperar y mostrar propiedades personalizadas
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Guarda el libro de trabajo
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


