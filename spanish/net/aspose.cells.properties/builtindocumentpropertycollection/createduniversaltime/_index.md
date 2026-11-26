---
title: "BuiltInDocumentPropertyCollection.CreatedUniversalTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la hora universal de la creación del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Obtiene o establece la hora universal de la creación del documento.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la propiedad CreatedUniversalTime
            DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
            workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
            
            // Mostrar la propiedad CreatedUniversalTime
            Console.WriteLine("Document created (UTC): " + 
                workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
            
            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


