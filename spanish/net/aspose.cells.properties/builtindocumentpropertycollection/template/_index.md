---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el nombre informativo de la plantilla del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Obtiene o establece el nombre informativo de la plantilla del documento.

```csharp
public string Template { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer la propiedad Template
            builtInProperties.Template = "Standard Template";

            // Establece otras propiedades básicas para la demostración
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Guarda el libro de trabajo
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


