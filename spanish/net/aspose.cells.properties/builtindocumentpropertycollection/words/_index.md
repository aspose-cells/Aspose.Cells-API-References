---
title: "BuiltInDocumentPropertyCollection.Words"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de palabras en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/words/
---
## BuiltInDocumentPropertyCollection.Words property

Representa una estimación del número de palabras en el documento.

```csharp
public int Words { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer la propiedad Words
            builtInProperties.Words = 250;

            // Agregar contenido a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample document");
            worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
            worksheet.Cells["A3"].PutValue("Total words will be set to 250");

            // Guarda el libro de trabajo
            workbook.Save("DocumentWithWordsProperty.xlsx");

            Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


