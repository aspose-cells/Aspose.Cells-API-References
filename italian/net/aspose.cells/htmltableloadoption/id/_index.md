---
title: "HtmlTableLoadOption.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Ottieni o imposta l'id della tabella da importare dall'html"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Ottieni o imposta l'id della tabella da importare da html

```csharp
public string Id { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configura le opzioni di caricamento della tabella
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Aggiungi opzioni di caricamento della tabella
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Carica il file HTML con le opzioni specificate
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


