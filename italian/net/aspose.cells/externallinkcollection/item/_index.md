---
title: "ExternalLinkCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalLinkCollection. Restituisce l'elemento ExternalLink all'indice specificato"
type: docs
url: /it/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Restituisce l'elemento [`ExternalLink`](../../externallink/) all'indice specificato.

```csharp
public ExternalLink this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con collegamenti esterni di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni collegamenti esterni
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // Accedi ai collegamenti esterni usando la proprietà Item
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                ExternalLink link = workbook.Worksheets.ExternalLinks[i];
                Console.WriteLine($"External Link {i + 1}:");
                Console.WriteLine($"- DataSource: {link.DataSource}");
                Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


