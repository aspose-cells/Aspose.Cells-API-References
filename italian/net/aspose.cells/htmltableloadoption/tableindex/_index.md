---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Ottieni o imposta l'indice della tabella da importare da html"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Ottieni o imposta l'indice della tabella da importare da html.

```csharp
public int TableIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Configura l'opzione di caricamento della tabella con TableIndex = 0 (prima tabella)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Aggiungi l'opzione di caricamento della tabella
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Carica il file HTML (sostituisci con il percorso reale)
            workbook = new Workbook("input.html", loadOptions);

            // Salva come file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


