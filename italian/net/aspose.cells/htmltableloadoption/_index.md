---
title: "Classe HtmlTableLoadOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.HtmlTableLoadOption. Rappresenta l'opzione durante l'importazione di una tabella da HTML"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Rappresenta l'opzione durante l'importazione di una tabella da HTML.

```csharp
public class HtmlTableLoadOption
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Ottieni o imposta l'id della tabella da importare da html |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) Ottieni o imposta il nome della tabella da importare da html |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Ottieni o imposta l'indice originale del foglio di lavoro nell'html. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Ottieni o imposta l'indice della tabella da importare da html. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Indica se generare oggetti elenco dalla tabella importata. Il valore predefinito è false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Ottieni o imposta l'indice di destinazione del foglio di lavoro dove la tabella deve essere collocata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea un'istanza di HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Crea un'istanza di HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Aggiungi HtmlTableLoadOption a HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Carica il file HTML nella cartella di lavoro con le opzioni di caricamento specificate
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


