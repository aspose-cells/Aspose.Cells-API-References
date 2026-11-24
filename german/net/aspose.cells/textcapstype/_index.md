---
title: "Enum TextCapsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextCapsType enum. Dieser Typ gibt die Kapitälchenarten des Textes an."
type: docs
url: /de/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Dieser Typ gibt die Großschreibungstypen des Textes an.

```csharp
public enum TextCapsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Kapitälchen |
| All | `1` | Alle Großbuchstaben auf den Text anwenden |
| Small | `2` | Kapitälchen auf den Text anwenden |

### Hinweise

Kann nur auf Diagramme und Formen angewendet werden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Zusätzlicher Code, um zu demonstrieren, wie die Instanz verwendet werden könnte
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Den Wert einer Zelle festlegen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Den Stil der Zelle abrufen
            Style style = cell.GetStyle();

            // Setze den Schriftkapitälchentyp auf Alle Großbuchstaben
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


