---
title: "HtmlTableLoadOption.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Ottieni o imposta il nome della tabella da importare da html"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Ottieni o imposta il nome della tabella da importare da html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi a HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella
            int index = tableLoadOptions.Add(0);

            // Accedi a HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Imposta la proprietà Name
            option.Name = "CustomerDataTable";

            // Carica un file HTML (sostituisci con il percorso reale del file)
            workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


