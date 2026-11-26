---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el estado del contenido del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Obtiene o establece el estado del contenido del documento.

```csharp
public string ContentStatus { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer propiedades de documento incorporadas incluyendo ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Guarda el libro de trabajo
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Mostrar la propiedad ContentStatus
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


