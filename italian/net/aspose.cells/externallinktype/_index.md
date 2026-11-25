---
title: "Enum ExternalLinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalLinkType enum. Rappresenta il tipo di collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Rappresenta il tipo di collegamento esterno.

```csharp
public enum ExternalLinkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DDELink | `0` | Rappresenta il collegamento DDE. |
| External | `1` | Rappresenta il collegamento esterno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Apri un file con collegamenti esterni
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Ottieni External Link
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Visualizza il tipo di collegamento esterno
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Modifica la fonte dati di External Link
            externalLink.DataSource = "d:\\link.xls";

            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Enum che rappresenta il tipo di collegamento esterno
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


