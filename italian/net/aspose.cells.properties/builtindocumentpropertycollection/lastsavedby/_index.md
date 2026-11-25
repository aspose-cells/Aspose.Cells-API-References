---
title: "BuiltInDocumentPropertyCollection.LastSavedBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il nome dell'ultimo autore"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedby/
---
## BuiltInDocumentPropertyCollection.LastSavedBy property

Ottiene o imposta il nome dell'ultimo autore.

```csharp
public string LastSavedBy { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta le proprietà integrate del documento includendo LastSavedBy
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";
            workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
            
            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
            
            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
            
            // Stampa la proprietà LastSavedBy
            Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


