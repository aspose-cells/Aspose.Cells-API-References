---
title: "DocumentProperty.ToDateTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DocumentProperty method. Devuelve el valor de la propiedad como DateTime en la zona horaria local"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Devuelve el valor de la propiedad como DateTime en la zona horaria local.

```csharp
public DateTime ToDateTime()
```

### Observaciones

Lanza una excepción si el tipo de propiedad no es PropertyType.Date.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtén la colección de propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agrega una propiedad datetime
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Obtén la propiedad y conviértela a DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Mostrar el resultado
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


