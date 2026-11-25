---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Ottieni o imposta l'indice di destinazione del foglio di lavoro dove deve essere posizionata la tabella"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Ottieni o imposta l'indice di destinazione del foglio di lavoro dove la tabella deve essere collocata.

```csharp
public int TargetSheetIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configura le opzioni di caricamento della tabella con TargetSheetIndex
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Aggiungi opzioni di caricamento della tabella
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Carica il file HTML con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica che le tabelle siano state caricate nei fogli corretti
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


