---
title: "Range.CopyValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Kopiert den Zellenwert aus einem Quellbereich"
type: docs
url: /de/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Kopiert den Zellenwert aus einem Quellbereich.

```csharp
public void CopyValue(Range range)
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
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Arbeitsblatt hinzu und erhalte das erste Arbeitsblatt
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Ein weiteres Arbeitsblatt für das Ziel hinzufügen
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Beispieldaten im Quellbereich erstellen
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Bereiche für Quelle und Ziel erstellen
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Werte vom Quellbereich zum Zielbereich kopieren
            rangeDest.CopyValue(rangeSrc);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


