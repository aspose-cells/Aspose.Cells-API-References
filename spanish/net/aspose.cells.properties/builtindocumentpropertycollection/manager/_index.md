---
title: "BuiltInDocumentPropertyCollection.Manager"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la propiedad manager"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Obtiene o establece la propiedad manager.

```csharp
public string Manager { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer propiedades principales del documento, incluido Manager
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
            builtInProperties.Company = "Aspose";

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx");

            Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


