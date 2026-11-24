---
title: "Enum FontSchemeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontSchemeType enum. Stellt den Schematyp der Schriftart dar."
type: docs
url: /de/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Stellt den Schema‑Typ der Schriftart dar.

```csharp
public enum FontSchemeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine |
| Major | `1` | Hauptschema. |
| Minor | `2` | Nebenschema. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Holen Sie die Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];
            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Cell cell = worksheet.Cells["A1"];
            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Hello Aspose!");

            // Greifen Sie auf die Schriftart des Zellstils zu
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Festlegen des Schriftart‑Schematyps auf Haupt
            font.SchemeType = FontSchemeType.Major;

            // Festlegen weiterer Schriftarteigenschaften zur Demonstration
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


