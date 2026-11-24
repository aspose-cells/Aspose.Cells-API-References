---
title: "Enum ShiftType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ShiftType‑Enum. Stellt die Verschiebungsoptionen dar, wenn ein Zellbereich gelöscht wird"
type: docs
url: /de/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Stellt die Verschiebungsoptionen beim Löschen eines Zellbereichs dar.

```csharp
public enum ShiftType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Down | `0` | Zellen nach unten verschieben. |
| Left | `1` | Zellen nach links verschieben. |
| None | `2` | Zellen nicht verschieben. |
| Right | `3` | Zellen nach rechts verschieben. |
| Up | `4` | Zellen nach oben verschieben. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Füge eine neue Zeile bei Index 1 ein und verschiebe die vorhandenen Zeilen nach unten
            worksheet.Cells.InsertRows(1, 1, true);

            // Setze einen Wert in der neu eingefügten Zeile
            worksheet.Cells["A1"].PutValue("New Item");

            // Lösche einen Zellbereich und verschiebe die Zellen nach oben
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Gib die verbleibenden Werte in der ersten Spalte aus
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


