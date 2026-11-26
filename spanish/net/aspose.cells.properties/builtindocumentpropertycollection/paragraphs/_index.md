---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de párrafos en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

Representa una estimación del número de párrafos en el documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Muestra el valor actual de Paragraphs (propiedad obsoleta)
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // Establece un nuevo valor para Paragraphs (propiedad obsoleta)
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // Agrega contenido para demostrar el efecto de la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // Guarda el libro de trabajo
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


