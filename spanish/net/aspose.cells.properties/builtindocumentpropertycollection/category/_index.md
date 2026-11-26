---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la categoría del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Obtiene o establece la categoría del documento.

```csharp
public string Category { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            var workbook = new Workbook();
            
            // Establecer propiedades de documento incorporadas
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // Guardar en flujo de memoria
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // Cargar el libro de trabajo nuevamente desde el flujo
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // Mostrar las propiedades
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


