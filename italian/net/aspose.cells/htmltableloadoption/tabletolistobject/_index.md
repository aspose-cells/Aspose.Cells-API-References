---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlTableLoadOption. Indica se generare oggetti elenco dalla tabella importata. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Indica se generare oggetti elenco dalla tabella importata. Il valore predefinito è false.

```csharp
public bool TableToListObject { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea le opzioni di caricamento HTML con TableToListObject abilitato
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Carica HTML con le opzioni specificate
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


