---
title: "BuiltInDocumentPropertyCollection.Comments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Ottiene o imposta i commenti del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Ottiene o imposta i commenti del documento.

```csharp
public string Comments { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Imposta la proprietà Comments
            properties.Comments = "This is a sample comment for demonstration.";
            
            // Visualizza la proprietà Comments
            Console.WriteLine("Document Comments: " + properties.Comments);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


