---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Indica si los hipervínculos en un documento están actualizados"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Indica si los hipervínculos en un documento están actualizados.

```csharp
public bool LinksUpToDate { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a la colección de propiedades de documento incorporada
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer la propiedad LinksUpToDate para indicar si los hipervínculos están actuales
            builtInProperties.LinksUpToDate = true;

            // Agregar un hipervínculo simple para demostrar la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Guarda el libro de trabajo
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


