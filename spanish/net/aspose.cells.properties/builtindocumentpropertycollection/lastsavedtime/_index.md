---
title: "BuiltInDocumentPropertyCollection.LastSavedTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la hora del último guardado en la zona horaria local"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedtime/
---
## BuiltInDocumentPropertyCollection.LastSavedTime property

Obtiene o establece la hora de la última guardada en la zona horaria local.

```csharp
public DateTime LastSavedTime { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer propiedades de documento incorporadas
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Mostrar la propiedad LastSavedTime
            Console.WriteLine("Last Saved Time: " + 
                workbook.BuiltInDocumentProperties.LastSavedTime);

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


