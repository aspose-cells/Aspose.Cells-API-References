---
title: "BuiltInDocumentPropertyCollection.Version"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa el número de versión de la aplicación que creó el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Representa el número de versión de la aplicación que creó el documento.

```csharp
public string Version { get; set; }
```

### Observaciones

Su formato es "00.0000", por ejemplo: 12.0000

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer algunas propiedades del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Acceder y mostrar la propiedad Version
            string version = workbook.BuiltInDocumentProperties.Version;
            Console.WriteLine("Document Version: " + version);
            
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


