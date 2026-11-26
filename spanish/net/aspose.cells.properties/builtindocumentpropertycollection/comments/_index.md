---
title: "BuiltInDocumentPropertyCollection.Comments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece los comentarios del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Obtiene o establece los comentarios del documento.

```csharp
public string Comments { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Establece la propiedad Comments
            properties.Comments = "This is a sample comment for demonstration.";
            
            // Muestra la propiedad Comments
            Console.WriteLine("Document Comments: " + properties.Comments);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


