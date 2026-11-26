---
title: "BuiltInDocumentPropertyCollection.LastSavedBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el nombre del último autor"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedby/
---
## BuiltInDocumentPropertyCollection.LastSavedBy property

Obtiene o establece el nombre del último autor.

```csharp
public string LastSavedBy { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer propiedades incorporadas del documento, incluido LastSavedBy
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";
            workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
            
            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
            
            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
            
            // Mostrar la propiedad LastSavedBy
            Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


