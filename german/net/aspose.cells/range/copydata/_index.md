---
title: "Range.CopyData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Kopiert Zellendaten einschließlich Formeln aus einem Quellbereich"
type: docs
url: /de/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Kopiert Zellen­daten (einschließlich Formeln) aus einem Quellbereich.

```csharp
public void CopyData(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | Range | Quell-[`Range`](../) Objekt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Hole das erste Arbeitsblatt und füge einige Daten hinzu
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Füge ein Zielarbeitsblatt hinzu
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Erstelle Quell- und Zielbereiche
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Kopiere Daten vom Quellbereich zum Zielbereich
            rangeDest.CopyData(rangeSrc);

            // Speichere die Arbeitsmappe
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


