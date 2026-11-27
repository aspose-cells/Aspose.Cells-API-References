---
title: "ErrorCheckOptionCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOptionCollection-egenskap. Hämtar ErrorCheckOption-objektet med angivet index"
type: docs
url: /sv/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Hämtar [`ErrorCheckOption`](../../errorcheckoption/) objektet med angivet index.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet |

### Returvärde

Returnerar [`ErrorCheckOption`](../../errorcheckoption/) objektet

### Exempel

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
            
            // Demonstrera användning av Item-egenskapen
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


