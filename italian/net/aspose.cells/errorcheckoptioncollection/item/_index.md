---
title: "ErrorCheckOptionCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorCheckOptionCollection. Ottiene l'oggetto ErrorCheckOption dato l'indice specificato."
type: docs
url: /it/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Ottiene l'oggetto [`ErrorCheckOption`](../../errorcheckoption/) dato l'indice specificato.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Valore di ritorno

Restituisce l'oggetto [`ErrorCheckOption`](../../errorcheckoption/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
            int optionIdx = opts.Add();
            
            // Dimostra l'uso della proprietà Item
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


