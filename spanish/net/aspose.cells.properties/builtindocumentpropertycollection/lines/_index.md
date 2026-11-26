---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de líneas en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Representa una estimación del número de líneas en el documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Mostrar el valor actual de Lines (estimación del número de líneas en el documento)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Establecer un nuevo valor para la propiedad Lines
            properties.Lines = 150;
            
            // Agregar contenido para demostrar el propósito de la propiedad
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Nota: La propiedad Lines es una estimación y no se actualizará automáticamente con el contenido real
            // Se utiliza principalmente con fines de metadatos de documentos
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


