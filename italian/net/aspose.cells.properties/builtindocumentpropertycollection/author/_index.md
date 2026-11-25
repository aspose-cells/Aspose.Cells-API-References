---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il nome dell'autore del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Ottiene o imposta il nome dell'autore del documento.

```csharp
public string Author { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta la proprietà author
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Visualizza la proprietà author
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // Salva la cartella di lavoro
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


