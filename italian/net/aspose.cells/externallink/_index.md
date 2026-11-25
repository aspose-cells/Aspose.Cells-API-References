---
title: "Classe ExternalLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalLink. Rappresenta un collegamento esterno in una cartella di lavoro"
type: docs
url: /it/net/aspose.cells/externallink/
---
## ExternalLink class

Rappresenta un collegamento esterno in una cartella di lavoro.

```csharp
public class ExternalLink
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Rappresenta la fonte dati del collegamento esterno. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indica se questo collegamento esterno è referenziato da altri. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indica se questo collegamento esterno è visibile in MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Rappresenta la fonte dati memorizzata del collegamento esterno. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Ottieni il tipo di percorso di questo collegamento esterno |
| [Type](../../aspose.cells/externallink/type/) { get; } | Ottiene il tipo di collegamento esterno. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Aggiunge un nome esterno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Apri un file con collegamenti esterni
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Ottieni External Link
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Visualizza le proprietà del collegamento esterno
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Modifica la fonte dati di External Link
            externalLink.DataSource = "d:\\linktest.xls";

            // Aggiungi un nome esterno al collegamento esterno
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Salva la cartella di lavoro
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


