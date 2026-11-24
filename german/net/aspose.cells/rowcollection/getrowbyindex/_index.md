---
title: "RowCollection.GetRowByIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RowCollection‑Methode. Gibt das Zeilenobjekt anhand der Position in der Liste zurück"
type: docs
url: /de/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Ermittelt das Zeilenobjekt anhand seiner Position in der Liste.

```csharp
public Row GetRowByIndex(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Die Position. |

### Rückgabewert

Das Row‑Objekt an der angegebenen Position.

### Beispiele

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
            
            // Zeile nach Index abrufen (0‑basiert)
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

### Siehe auch

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


