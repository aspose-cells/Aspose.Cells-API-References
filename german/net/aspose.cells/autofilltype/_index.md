---
title: "Enum AutoFillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AutoFillType-Enum. Stellt den Autoausfülltyp dar."
type: docs
url: /de/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Stellt den Auto‑Ausfülltyp dar.

```csharp
public enum AutoFillType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Copy | `1` | Kopiert den Wert und das Format des Quellbereichs in den Zielbereich. |
| Default | `0` | Füllt den Zielbereich automatisch mit dem Wert und dem Format. |
| Formats | `3` | Kopiert nur das Format des Quellbereichs in den Zielbereich. |
| Series | `2` | Erweitert den Wert im Quellbereich in den Zielbereich in Form einer Serie und kopiert das Format in den Zielbereich. |
| Values | `4` | Kopiert nur den Wert des Quellbereichs in den Zielbereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich (A1:A10) und fülle ihn mit einigen Werten.
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Erstelle einen Zielbereich (B1:B10).
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Serientyp-Fehler, Ticket wurde erstellt.
            // Verwende die AutoFill-Methode mit AutoFillType.Series, um den Zielbereich zu füllen.
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Verwende die AutoFill-Methode mit AutoFillType.Copy, um den Zielbereich zu füllen.
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


