---
title: "BuiltInDocumentPropertyCollection.NameOfApplication"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el nombre de la aplicación"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Obtiene o establece el nombre de la aplicación.

```csharp
public string NameOfApplication { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la propiedad NameOfApplication
            workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
            
            // Mostrar la propiedad NameOfApplication
            Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
            
            // Guarda el libro de trabajo
            workbook.Save("output.ods");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


