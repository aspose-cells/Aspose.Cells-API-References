---
title: "BuiltInDocumentPropertyCollection.ContentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el tipo de contenido del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

Obtiene o establece el tipo de contenido del documento.

```csharp
public string ContentType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la propiedad ContentType
            workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";

            // Mostrar la propiedad ContentType
            Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


