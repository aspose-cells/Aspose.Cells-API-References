---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el idioma del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Obtiene o establece el idioma del documento.

```csharp
public string Language { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a la colección de propiedades de documento incorporada
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establece la propiedad language
            builtInProperties.Language = "en-US";

            // Establece otras propiedades básicas para la demostración
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Guarda el libro de trabajo
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


