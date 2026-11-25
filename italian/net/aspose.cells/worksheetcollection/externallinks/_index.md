---
title: "WorksheetCollection.ExternalLinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Rappresenta i collegamenti esterni in una cartella di lavoro"
type: docs
url: /it/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Rappresenta i collegamenti esterni in una cartella di lavoro.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro sorgente con collegamento esterno
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Crea una cartella di lavoro di destinazione
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Imposta la fonte dati del collegamento esterno
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Salva la cartella di lavoro
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Pulisci
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Vedi anche

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


