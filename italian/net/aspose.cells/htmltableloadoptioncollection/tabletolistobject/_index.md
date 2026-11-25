---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "HtmlTableLoadOptionCollection proprietà. Indica se generare oggetti elenco dalle tabelle importate. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Indica se generare oggetti elenco dalle tabelle importate. Il valore predefinito è false.

```csharp
public bool TableToListObject { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();

            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi all'istanza di HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Imposta la proprietà TableToListObject per convertire le tabelle HTML in ListObjects
            tableLoadOptions.TableToListObject = true;

            // Aggiungi una tabella da convertire in ListObject per indice
            tableLoadOptions.Add(0);

            // Carica un file HTML nella cartella di lavoro usando le opzioni di caricamento
            workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


