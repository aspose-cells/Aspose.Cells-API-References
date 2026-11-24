---
title: "Cells.GetRowHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Höhe einer angegebenen Zeile in der Einheit Zoll zurück"
type: docs
url: /de/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Gibt die Höhe einer angegebenen Zeile in Zoll zurück.

```csharp
public double GetRowHeightInch(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Höhe der Zeile

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze die Zeilenhöhe in Zoll für Zeile 5
            cells.SetRowHeightInch(5, 1.5);

            // Hole die Zeilenhöhe in Zoll für Zeile 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Gib das Ergebnis aus
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


