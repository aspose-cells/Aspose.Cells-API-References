---
title: "Klasse CellWatch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellWatch Klasse. Stellt das Cell Watch-Element im Überwachungsfenster dar."
type: docs
url: /de/net/aspose.cells/cellwatch/
---
## CellWatch class

Stellt ein Cell Watch Item im 'Watch-Fenster' dar.

```csharp
public class CellWatch
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CellWatch](cellwatch/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Ermittelt und setzt den Namen der Zelle. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Ermittelt und setzt die Spalte der Zelle. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Ermittelt und setzt die Zeile der Zelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            // Holen Sie das erste Arbeitsblatt.
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie das Cell Watch-Element in das Überwachungsfenster ein
            int watchIndex = sheet.CellWatches.Add("B2");

            // Rufen Sie das CellWatch-Objekt ab
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Eigenschaften festlegen
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Speichere die Arbeitsmappe
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


