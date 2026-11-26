---
title: "DocumentProperty.ToDouble"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentProperty. Devuelve el valor de la propiedad como double"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Devuelve el valor de la propiedad como double.

```csharp
public double ToDouble()
```

### Observaciones

Lanza una excepción si el tipo de la propiedad no es PropertyType.Float.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtén la colección de propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agregue una propiedad numérica
            customProperties.Add("Rating", 4.75);

            // Obtenga la propiedad y conviértala a double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Mostrar el resultado
            Console.WriteLine($"Rating: {ratingValue}");

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


