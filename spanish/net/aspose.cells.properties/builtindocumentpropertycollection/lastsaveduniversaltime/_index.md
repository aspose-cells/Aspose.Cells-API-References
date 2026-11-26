---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la hora universal del último guardado"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Obtiene o establece la hora universal de la última guardada.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer la propiedad LastSavedUniversalTime
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Mostrar el valor establecido
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Guarda el libro de trabajo
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


