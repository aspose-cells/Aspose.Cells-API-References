---
title: "BuiltInDocumentPropertyCollection.CreatedTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la data di creazione del documento nel fuso orario locale"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Ottiene o imposta la data di creazione del documento nel fuso orario locale.

```csharp
public DateTime CreatedTime { get; set; }
```

### Osservazioni

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà CreatedTime all'ora corrente
            DateTime currentTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
            
            // Salva la cartella di lavoro
            string outputPath = "output_CreatedTimeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook(outputPath);
            DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
            
            Console.WriteLine("Original CreatedTime: " + currentTime);
            Console.WriteLine("Loaded CreatedTime: " + loadedTime);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


