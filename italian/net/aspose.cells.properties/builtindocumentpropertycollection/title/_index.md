---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Ottiene o imposta il titolo del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Ottiene o imposta il titolo del documento.

```csharp
public string Title { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la proprietà Title
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Visualizza la proprietà Title
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


