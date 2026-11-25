---
title: "BuiltInDocumentPropertyCollection.Words"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta una stima del numero di parole nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/words/
---
## BuiltInDocumentPropertyCollection.Words property

Rappresenta una stima del numero di parole nel documento.

```csharp
public int Words { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà Words
            builtInProperties.Words = 250;

            // Aggiungi del contenuto al foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample document");
            worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
            worksheet.Cells["A3"].PutValue("Total words will be set to 250");

            // Salva la cartella di lavoro
            workbook.Save("DocumentWithWordsProperty.xlsx");

            Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


