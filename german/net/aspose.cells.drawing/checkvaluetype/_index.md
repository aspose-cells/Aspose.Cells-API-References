---
title: "Aufzählung CheckValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.CheckValueType Enum. Stellt den Prüfwerttyp des Kontrollkästchens dar"
type: docs
url: /de/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Stellt den Prüfwerttyp des Kontrollkästchens dar.

```csharp
public enum CheckValueType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| UnChecked | `0` | Nicht markiert |
| Checked | `1` | Markiert |
| Mixed | `2` | Gemischt |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Kontrollkästchen zum Arbeitsblatt hinzu
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Rufe die Kontrollkästchen ab und setze deren Eigenschaften
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Setze die Werte der Kontrollkästchen und deren Markierungsstatus
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Verknüpfe Kontrollkästchen mit Zellen
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Gib die Zellwerte aus, um die Verknüpfung zu demonstrieren
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


