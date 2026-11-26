---
title: "BuiltInDocumentPropertyCollection.DocumentVersion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa la versión del archivo"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

Representa la versión del archivo.

```csharp
public string DocumentVersion { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la propiedad de versión del documento
            workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
            
            // Mostrar la versión del documento
            Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
            
            // Guarda el libro de trabajo
            workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


