---
title: "DocumentProperty.ToInt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentProperty. Devuelve el valor de la propiedad como entero"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Devuelve el valor de la propiedad como integer.

```csharp
public int ToInt()
```

### Observaciones

Lanza una excepción si el tipo de propiedad no es PropertyType.Number.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la colección de propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agregar una propiedad personalizada numérica
            customProperties.Add("Revision", 5);

            // Obtén la propiedad y conviértela a int usando ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Mostrar el resultado
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


