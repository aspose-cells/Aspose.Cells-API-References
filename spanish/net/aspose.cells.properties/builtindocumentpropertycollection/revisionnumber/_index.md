---
title: "BuiltInDocumentPropertyCollection.RevisionNumber"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el número de revisión del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

Obtiene o establece el número de revisión del documento.

```csharp
public string RevisionNumber { get; set; }
```

### Observaciones

Aspose.Cells no actualiza esta propiedad cuando modificas el documento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establezca la propiedad RevisionNumber
            workbook.BuiltInDocumentProperties.RevisionNumber = "1";
            
            // Muestre el RevisionNumber
            Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


