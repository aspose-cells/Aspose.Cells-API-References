---
title: "Row.GetCellByIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Gibt die Zelle anhand eines bestimmten Indexes in der Zellen‑Sammlung dieser Zeile zurück."
type: docs
url: /de/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Ruft die Zelle anhand eines bestimmten Indexes in der Zellsammlung dieser Zeile ab.

```csharp
public Cell GetCellByIndex(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index (Position) der Zelle in der Zellen‑Sammlung dieser Zeile. |

### Rückgabewert

Das Cell‑Objekt an der angegebenen Position.

### Hinweise

Um alle Zellen sequenziell ohne Änderungen zu durchlaufen, liefert die Verwendung von [`GetEnumerator`](../getenumerator/) eine bessere Leistung als die Verwendung dieser Methode, um Zellen einzeln abzurufen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Daten zu Zellen in der ersten Zeile hinzufügen
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Erste Zeile abrufen
            Row row = worksheet.Cells.Rows[0];

            // Demonstration von GetCellByIndex mit Int32‑Parameter
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


