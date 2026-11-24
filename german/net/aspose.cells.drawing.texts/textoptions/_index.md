---
title: "Klasse TextOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextOptions Klasse. Stellt die Textoptionen dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Stellt die Textoptionen dar.

```csharp
public class TextOptions : Font
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Liest und setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Liest und setzt den Kapitälchentyp für Texte der Form. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Stellt den Zeichensatz dar.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Liest oder setzt die Farbe der Schriftart.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Liest und setzt die doppelte Größe der Schriftart.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Liest und setzt den FarEast-Namen. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Stellt das Füllformat des Textes dar. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Schrift fett ist.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Schrift kursiv ist.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Gibt an, ob die Höhennormalisierung auf den Textlauf angewendet werden soll. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Schrift einmal durchgestrichen ist.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Schrift tiefgestellt ist.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Schrift hochgestellt ist.(Geerbt von [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Gibt die minimale Schriftgröße an, bei der für diesen Textlauf Kerning zwischen Zeichen erfolgt. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Liest und setzt die Sprache der Benutzeroberfläche. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Liest und setzt den lateinischen Namen. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Liest und setzt den Namen der Form. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Stellt das Umrissformat des Textes dar. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Liest und setzt den Schematyp der Schrift.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Liest und setzt den Skriptversatz in Prozent(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Stellt ein [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Liest oder setzt die Größe der Schrift.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Gibt den Abstand zwischen Zeichen innerhalb eines Textlaufs an. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Liest den Durchstreichungstyp des Textes.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Liest und setzt die Themenfarbe.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Liest oder setzt den Unterstreichungstyp der Schrift.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Liest oder setzt die Farbe der Unterstreichung. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Prüft, ob zwei Schriften gleich sind.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Setzt Namen und Schema der Schrift.(Inherited from [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Gibt einen String zurück, der das aktuelle Zellobjekt darstellt.(Inherited from [`Font`](../../aspose.cells/font/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügt dem Arbeitsblatt eine Form mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Fügt der Form Text hinzu und erhält TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Setze Textoptionen
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


