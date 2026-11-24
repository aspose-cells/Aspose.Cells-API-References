---
title: "Aufzählung FontUnderlineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontUnderlineType enum. Enumeriert die Schriftunterstreichungsarten."
type: docs
url: /de/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Enumeriert die Schriftunterstreichungsarten.

```csharp
public enum FontUnderlineType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Stellt keine Unterstreichung dar. |
| Single | `1` | Stellt eine einfache Unterstreichung dar. |
| Double | `2` | Stellt eine doppelte Unterstreichung dar. |
| Accounting | `3` | Stellt eine einfache Buchhaltungsunterstreichung dar. |
| DoubleAccounting | `4` | Stellt eine doppelte Buchhaltungsunterstreichung dar. |
| Dash | `5` | Stellt eine gestrichelte Unterstreichung dar |
| DashDotDotHeavy | `6` | Stellt eine dicke Strich-Punkt-Punkt‑Unterstreichung dar |
| DashDotHeavy | `7` | Stellt eine dicke Strich-Punkt-Unterstreichung dar |
| DashedHeavy | `8` | Stellt eine dicke gestrichelte Unterstreichung dar |
| DashLong | `9` | Stellt eine lange gestrichelte Unterstreichung dar |
| DashLongHeavy | `10` | Stellt eine dicke lange gestrichelte Unterstreichung dar |
| DotDash | `11` | Stellt eine Strich-Punkt-Unterstreichung dar |
| DotDotDash | `12` | Stellt eine Strich-Punkt-Punkt-Unterstreichung dar |
| Dotted | `13` | Stellt eine gepunktete Unterstreichung dar |
| DottedHeavy | `14` | Stellt eine dicke gepunktete Unterstreichung dar |
| Heavy | `15` | Stellt eine dicke Unterstreichung dar |
| Wave | `16` | Stellt eine Wellenunterstreichung dar |
| WavyDouble | `17` | Stellt eine doppelte Wellenunterstreichung dar |
| WavyHeavy | `18` | Stellt eine schwere Wellenunterstreichung dar |
| Words | `19` | Stellt die Unterstreichung von Nicht-Leerzeichen-Zeichen dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Cell cell = worksheet.Cells["A1"];
            
            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Hello Aspose!");

            // Ermitteln Sie den Stil der Zelle
            Style style = cell.GetStyle();
            
            // Setzen Sie den Unterstreichungstyp der Schrift auf einfache Unterstreichung
            style.Font.Underline = FontUnderlineType.Single;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


