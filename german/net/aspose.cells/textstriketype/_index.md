---
title: "Aufzählung TextStrikeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextStrikeType Enum. Dieser Typ gibt den Durchstreichungstyp an."
type: docs
url: /de/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Dieser Typ gibt den Durchstreichungstyp an.

```csharp
public enum TextStrikeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Single | `0` | Ein einfacher Durchstrich, der auf den Text angewendet wird. |
| Double | `1` | Ein doppelter Durchstrich, der auf den Text angewendet wird. Funktioniert nur für den Text von Formen oder Diagrammen. |
| None | `2` | Kein Durchstrich wird auf den Text angewendet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Holen Sie die Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];
            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Cell cell = worksheet.Cells["A1"];
            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Hello Aspose!");

            // Zugriff auf die Schriftart der Zelle
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Festlegen des Durchstreichungstyps auf Einzel
            font.StrikeType = TextStrikeType.Single;

            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


