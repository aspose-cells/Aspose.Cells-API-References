---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece las palabras clave del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Obtiene o establece las palabras clave del documento.

```csharp
public string Keywords { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la propiedad Keywords
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Guarda el libro de trabajo
            workbook.Save("output_keywords.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar la propiedad Keywords
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Mostrar la propiedad Keywords
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


