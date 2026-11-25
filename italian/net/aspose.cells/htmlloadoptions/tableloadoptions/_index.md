---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Ottieni l'istanza HtmlTableLoadOptionCollection"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Ottieni l'istanza di HtmlTableLoadOptionCollection

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Aggiungi le opzioni di caricamento della tabella per indice
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Aggiungi opzioni di caricamento della tabella per ID
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Carica il file HTML con le opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Salva l'output
            workbook.Save("output.xlsx");
            
            // Cancella e aggiungi nuove opzioni di caricamento della tabella
            loadOptions.TableLoadOptions.Clear();
            
            // Aggiungi opzioni di caricamento della tabella con mappatura dell'indice del foglio
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Aggiungi opzioni di caricamento della tabella con ID e mappatura del foglio
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Carica e salva nuovamente con nuove opzioni
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


