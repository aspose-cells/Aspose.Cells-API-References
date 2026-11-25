---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta le parole chiave del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Ottiene o imposta le parole chiave del documento.

```csharp
public string Keywords { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà Keywords
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Salva la cartella di lavoro
            workbook.Save("output_keywords.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare la proprietà Keywords
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Visualizza la proprietà Keywords
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


