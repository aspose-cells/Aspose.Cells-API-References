---
title: "ErrorCheckOptionCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOptionCollection Eigenschaft. Gibt das ErrorCheckOption-Objekt anhand des angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Gibt das [`ErrorCheckOption`](../../errorcheckoption/)-Objekt anhand des angegebenen Index zurück.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Rückgabewert

Gibt das [`ErrorCheckOption`](../../errorcheckoption/)-Objekt zurück

### Beispiele

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
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


