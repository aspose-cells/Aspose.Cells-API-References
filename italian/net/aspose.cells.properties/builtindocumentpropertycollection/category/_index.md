---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la categoria del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Ottiene o imposta la categoria del documento.

```csharp
public string Category { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            var workbook = new Workbook();
            
            // Imposta le proprietà integrate del documento
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // Salva su stream di memoria
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // Carica nuovamente la cartella di lavoro dallo stream
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // Visualizza le proprietà
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


