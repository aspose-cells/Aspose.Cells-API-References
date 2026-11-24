---
title: "Range.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range‑Eigenschaft. Gibt den Wert des Bereichs zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/range/value/
---
## Range.Value property

Liefert und setzt den Wert des Bereichs.

```csharp
public object Value { get; set; }
```

### Hinweise

Wenn der Bereich mehrere Zellen enthält, sollte das zurückgegebene/angewendete Objekt ein zweidimensionales Array-Objekt sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich, der bei A1 beginnt und 3 × 3 Zellen umfasst
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Setze ein 2D-Array als Wert für den Bereich
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Speichere die Arbeitsmappe
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


