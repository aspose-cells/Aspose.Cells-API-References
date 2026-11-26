---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el nombre del autor del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Obtiene o establece el nombre del autor del documento.

```csharp
public string Author { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la propiedad author
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Mostrar la propiedad del autor
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

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


