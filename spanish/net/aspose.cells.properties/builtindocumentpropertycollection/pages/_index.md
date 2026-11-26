---
title: "BuiltInDocumentPropertyCollection.Pages"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de páginas en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/pages/
---
## BuiltInDocumentPropertyCollection.Pages property

Representa una estimación del número de páginas en el documento.

```csharp
public int Pages { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establezca la propiedad Pages
            builtInProperties.Pages = 10;

            // Agregar una hoja de cálculo y algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page Count Demonstration");
            worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");

            // Guarda el libro de trabajo
            workbook.Save("DocumentPagesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


