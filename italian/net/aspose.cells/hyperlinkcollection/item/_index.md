---
title: "HyperlinkCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HyperlinkCollection. Ottiene l'elemento Hyperlink all'indice specificato"
type: docs
url: /it/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Ottiene l'elemento [`Hyperlink`](../../hyperlink/) all'indice specificato.

```csharp
public Hyperlink this[int index] { get; }
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
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento ipertestuale alla cella A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Accedi al primo collegamento ipertestuale usando la proprietà Item e imposta il testo visualizzato
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Imposta lo stile del collegamento ipertestuale (testo blu sottolineato)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


