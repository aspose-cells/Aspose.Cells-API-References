---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta la proprietà hyperlinkbase"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Ottiene o imposta la proprietà hyperlinkbase.

```csharp
public string HyperlinkBase { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta la proprietà HyperlinkBase
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Imposta un'altra proprietà per dimostrazione
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Salva la cartella di lavoro
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Stampa le proprietà sulla console
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


