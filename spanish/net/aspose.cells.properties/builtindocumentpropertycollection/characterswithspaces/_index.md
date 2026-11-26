---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de caracteres, incluidos los espacios, en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

Representa una estimación del número de caracteres (incluidos los espacios) en el documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Mostrar el valor actual de CharactersWithSpaces
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Establecer un nuevo valor para CharactersWithSpaces
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // Agrega contenido para demostrar el efecto de la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // Guarda el libro de trabajo
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


