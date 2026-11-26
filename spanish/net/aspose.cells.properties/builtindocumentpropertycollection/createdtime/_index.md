---
title: "BuiltInDocumentPropertyCollection.CreatedTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la fecha de creación del documento en la zona horaria local"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Obtiene o establece la fecha de creación del documento en la zona horaria local.

```csharp
public DateTime CreatedTime { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establezca la propiedad CreatedTime a la hora actual
            DateTime currentTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
            
            // Guarda el libro de trabajo
            string outputPath = "output_CreatedTimeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook(outputPath);
            DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
            
            Console.WriteLine("Original CreatedTime: " + currentTime);
            Console.WriteLine("Loaded CreatedTime: " + loadedTime);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


