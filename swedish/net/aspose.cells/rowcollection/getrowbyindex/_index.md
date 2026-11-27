---
title: "RowCollection.GetRowByIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RowCollection‑metod. Hämtar rad‑objektet efter positionen i listan"
type: docs
url: /sv/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Hämtar radobjektet efter positionen i listan.

```csharp
public Row GetRowByIndex(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Positionen. |

### Returvärde

Row‑objektet vid angiven position.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hämta rad efter index (0‑baserat)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### Se även

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


