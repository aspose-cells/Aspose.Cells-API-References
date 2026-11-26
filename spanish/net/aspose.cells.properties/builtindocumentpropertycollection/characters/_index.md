---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de caracteres en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

Representa una estimación del número de caracteres en el documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Muestra el valor actual de Characters (propiedad obsoleta)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // Establece un nuevo valor para Characters (propiedad obsoleta)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // Agrega contenido para demostrar el efecto de la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // Guarda el libro de trabajo
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


