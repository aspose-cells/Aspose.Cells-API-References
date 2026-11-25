---
title: "Row.IsHeightMatched"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è automatica senza un valore di altezza personalizzato impostato dall'utente"
type: docs
url: /it/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è "automatica" senza un valore di altezza personalizzato impostato dall'utente.

```csharp
public bool IsHeightMatched { get; set; }
```

### Osservazioni

Quando questa proprietà è true, se il contenuto di questa riga cambia, generalmente l'altezza della riga deve essere ricalcolata (ad esempio tramite [`AutoFitRows`](../../worksheet/autofitrows/)) per ottenere lo stesso risultato di quanto mostrato in MS Excel quando si apre la cartella di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio e stile per dimostrare la corrispondenza dell'altezza della riga
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Applica l'andata a capo automatico per forzare la regolazione dell'altezza
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Adatta automaticamente la riga per corrispondere all'altezza del contenuto
            worksheet.AutoFitRow(0);
            
            // Verifica se l'altezza della riga corrisponde al suo contenuto
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


