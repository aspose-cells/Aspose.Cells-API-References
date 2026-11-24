---
title: "Range.GetCellOrNull"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt das Cell-Objekt oder null in diesem Bereich zurück"
type: docs
url: /de/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Liefert das [`Cell`](../../cell/) Objekt oder null in diesem Bereich.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | Int32 | Spaltenversatz in diesem Bereich, nullbasiert. |

### Rückgabewert

[`Cell`](../../cell/) object.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Fülle einige Daten in den Bereich ein
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Demonstriere GetCellOrNull mit Int32-Parametern
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Versuche, eine Zelle außerhalb des Bereichs zu erhalten (sollte null zurückgeben)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


