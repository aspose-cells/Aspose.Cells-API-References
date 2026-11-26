---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la fecha en que el documento se imprimió por última vez en la zona horaria local"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Obtiene o establece la fecha en que el documento se imprimió por última vez en la zona horaria local.

```csharp
public DateTime LastPrinted { get; set; }
```

### Observaciones

Si el documento nunca se imprimió, esta propiedad devolverá DateTime.MinValue.

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer propiedades de documento incorporadas
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Mostrar la propiedad LastPrinted
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


