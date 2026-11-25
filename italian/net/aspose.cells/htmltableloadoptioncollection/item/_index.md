---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOptionCollection. Ottiene l'elemento HtmlTableLoadOption all'indice specificato"
type: docs
url: /it/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Ottiene l'elemento [`HtmlTableLoadOption`](../../htmltableloadoption/) all'indice specificato.

```csharp
public HtmlTableLoadOption this[int index] { get; }
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
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella
            int index1 = tableLoadOptions.Add(0);

            // Accedi all'HtmlTableLoadOption usando la proprietà Item
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Configura l'opzione di caricamento della tabella
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Carica il file HTML con le opzioni configurate
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


