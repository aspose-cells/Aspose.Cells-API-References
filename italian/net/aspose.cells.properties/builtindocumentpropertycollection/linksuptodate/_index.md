---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Indica se i collegamenti ipertestuali in un documento sono aggiornati"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Indica se i collegamenti ipertestuali in un documento sono aggiornati.

```csharp
public bool LinksUpToDate { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alla collezione delle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà LinksUpToDate per indicare se i collegamenti ipertestuali sono attuali
            builtInProperties.LinksUpToDate = true;

            // Aggiungi un collegamento ipertestuale semplice per dimostrare la proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Salva la cartella di lavoro
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


