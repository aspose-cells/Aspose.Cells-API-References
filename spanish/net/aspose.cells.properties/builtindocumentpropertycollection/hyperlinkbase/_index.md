---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la propiedad hyperlinkbase"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Obtiene o establece la propiedad hyperlinkbase.

```csharp
public string HyperlinkBase { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la propiedad HyperlinkBase
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Establecer alguna otra propiedad para demostración
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Guarda el libro de trabajo
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Mostrar las propiedades en la consola
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


