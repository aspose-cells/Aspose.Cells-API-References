---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Representa una estimación del número de bytes en el documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

Representa una estimación del número de bytes en el documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Muestre el valor actual de Bytes (estimación del tamaño del documento)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // Agregue contenido para afectar el tamaño
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // Actualice la propiedad Bytes manualmente (aunque normalmente se calcularía automáticamente)
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // Guarde el libro de trabajo para ver la propiedad en el archivo guardado
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


