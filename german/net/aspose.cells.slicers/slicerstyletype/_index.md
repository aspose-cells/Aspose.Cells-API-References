---
title: "Enum SlicerStyleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Slicers.SlicerStyleType‑Enum. Gibt den Stil der Slicer‑Ansicht an"
type: docs
url: /de/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Gibt den Stil der Slicer‑Ansicht an

```csharp
public enum SlicerStyleType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | eingebauter heller Stil eins |
| SlicerStyleLight2 | `1` | eingebauter heller Stil zwei |
| SlicerStyleLight3 | `2` | eingebauter heller Stil drei |
| SlicerStyleLight4 | `3` | eingebauter heller Stil vier |
| SlicerStyleLight5 | `4` | eingebauter heller Stil fünf |
| SlicerStyleLight6 | `5` | eingebauter heller Stil sechs |
| SlicerStyleOther1 | `6` | eingebauter anderer Stil eins |
| SlicerStyleOther2 | `7` | eingebauter anderer Stil zwei |
| SlicerStyleDark1 | `8` | eingebauter dunkler Stil eins |
| SlicerStyleDark2 | `9` | eingebauter dunkler Stil zwei |
| SlicerStyleDark3 | `10` | eingebauter dunkler Stil drei |
| SlicerStyleDark4 | `11` | eingebauter dunkler Stil vier |
| SlicerStyleDark5 | `12` | eingebauter dunkler Stil fünf |
| SlicerStyleDark6 | `13` | eingebauter dunkler Stil sechs |
| Custom | `14` | benutzerdefinierter Stil, derzeit nicht unterstützt |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Füge Slicer hinzu
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Slicer‑Stil festlegen
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Speichere die Arbeitsmappe
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


