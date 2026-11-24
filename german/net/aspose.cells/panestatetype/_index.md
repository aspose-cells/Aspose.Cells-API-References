---
title: "Enum PaneStateType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PaneStateType‑Enum. Stellt den Zustand des Tabellenblattsbereichs dar"
type: docs
url: /de/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Stellt den Zustand des Tabellenblattsbereichs dar.

```csharp
public enum PaneStateType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Frozen | `0` | Bereiche sind eingefroren, waren jedoch vorher nicht eingefroren. |
| FrozenSplit | `1` | Bereiche sind eingefroren und wurden vor dem Einfrieren geteilt. |
| Split | `2` | Bereiche sind geteilt, aber nicht eingefroren. |
| Normal | `3` | Bereiche sind weder eingefroren noch geteilt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze einige Beispieldaten im Arbeitsblatt.
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Friere Bereiche bei Zelle B2 ein.
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Überprüfe den Zustand des Bereichs.
            PaneStateType paneState = worksheet.PaneState;

            // Gib den Zustand des Bereichs aus.
            Console.WriteLine("Current Pane State: " + paneState);

            // Speichere die Arbeitsmappe
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


