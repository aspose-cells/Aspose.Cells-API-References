---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Ottiene o imposta lo stato del contenuto del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Ottiene o imposta lo stato del contenuto del documento.

```csharp
public string ContentStatus { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le proprietà integrate del documento includendo ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Salva la cartella di lavoro
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Visualizza la proprietà ContentStatus
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


