---
title: "Klasse Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Font-Klasse. Kapselt das in einer Tabellenkalkulation verwendete Schriftobjekt"
type: docs
url: /de/net/aspose.cells/font/
---
## Font class

Kapselt das Schriftobjekt, das in einer Tabellenkalkulation verwendet wird.

```csharp
public class Font
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Liest und setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Ruft den Text‑Großschreibungstyp ab und legt ihn fest. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Stellt den Zeichensatz dar. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Ruft die Farbe der Schrift ab oder legt sie fest. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Ruft die doppelte Größe der Schrift ab und legt sie fest. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift fett ist. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift kursiv ist. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Gibt an, ob die Normalisierung der Höhe, die auf den Textlauf angewendet werden soll, aktiv ist. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift einfach durchgestrichen ist. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift tiefgestellt ist. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift hochgestellt ist. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Ruft den Namen des `Font` ab oder legt ihn fest. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Liest und setzt den Schematyp der Schriftart. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Liest und setzt den Skriptversatz, in Prozent. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Liest oder setzt die Größe der Schriftart. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Liest den Durchstreichungstyp des Textes. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Liest und setzt die Themenfarbe. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Liest oder setzt den Unterstreichungstyp der Schriftart. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Prüft, ob zwei Schriftarten gleich sind. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Setzt Name und Schema der Schriftart. |
| override [ToString](../../aspose.cells/font/tostring/)() | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Hello Aspose!");

            // Zugriff auf das Schriftobjekt des Zellstils
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Setzen des Schriftartnamens auf "Times New Roman"
            font.Name = "Times New Roman";

            // Setzen der Schriftgröße auf 14
            font.Size = 14;

            // Setzen der Schriftfarbe auf Rot
            font.Color = Color.Red;

            // Setzen zusätzlicher Schriftarteigenschaften
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Die Excel-Datei speichern
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


