---
title: "Range.GetOffset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt den Range-Bereich anhand des Offsets zurück"
type: docs
url: /de/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Gibt den [`Range`](../)-Bereich anhand des Offsets zurück.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Zeilenversatz in diesem Bereich, nullbasiert. |
| columnOffset | Int32 | Spaltenversatz in diesem Bereich, nullbasiert. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Erstelle den initialen Bereich
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Erhalte den Offset-Bereich
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


