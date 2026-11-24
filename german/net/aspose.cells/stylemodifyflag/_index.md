---
title: "Aufzählung StyleModifyFlag"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.StyleModifyFlag-Enum. Die modifizierten Stil-Flags"
type: docs
url: /de/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Die modifizierten Stil-Flags.

```csharp
public enum StyleModifyFlag
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LeftBorder | `256` | Gibt an, ob der linke Rand für den Stil geändert wurde. |
| RightBorder | `512` | Gibt an, ob der rechte Rand für den Stil geändert wurde. |
| TopBorder | `1024` | Gibt an, ob der obere Rand für den Stil geändert wurde. |
| BottomBorder | `2048` | Gibt an, ob der untere Rand für den Stil geändert wurde. |
| DiagonalDownBorder | `4096` | Gibt an, ob der diagonale‑abwärts Rand für den Stil geändert wurde. |
| DiagonalUpBorder | `8192` | Gibt an, ob der diagonale‑aufwärts Rand für den Stil geändert wurde. |
| HorizontalBorder | `32` | Gibt an, ob der horizontale Rand für den Stil geändert wurde. Nur für dynamische Stile, wie z. B. bedingte Formatierung. |
| VerticalBorder | `64` | Gibt an, ob der vertikale Rand für den Stil geändert wurde. Nur für dynamische Stile, wie z. B. bedingte Formatierung. |
| SideBorders | `3840` | Gibt die vier Seitenränder an: LeftBorder, RightBorder, TopBorder und BottomBorder. |
| Diagonal | `12288` | Gibt diagonale Ränder an: DiagonalDownBorder und DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Gibt die Ränder des dynamischen Stils an: HorizontalBorder und VerticalBorder. |
| Borders | `16224` | Gibt an, ob einer oder mehrere Ränder (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) für den Stil geändert wurden. |
| NumberFormat | `16384` | Gibt an, ob das Zahlenformat geändert wurde. |
| HorizontalAlignment | `32768` | Gibt an, ob die horizontale Ausrichtung geändert wurde. |
| VerticalAlignment | `65536` | Gibt an, ob die vertikale Ausrichtung geändert wurde. |
| Indent | `131072` | Gibt an, ob die Einzugs‑Eigenschaft geändert wurde. |
| Rotation | `262144` | Gibt an, ob die Drehungs‑Eigenschaft geändert wurde. |
| WrapText | `524288` | Gibt an, ob die Zeilenumbruch‑Eigenschaft geändert wurde. |
| ShrinkToFit | `1048576` | Gibt an, ob die Schrumpfen‑zum‑Anpassen‑Eigenschaft geändert wurde. |
| TextDirection | `2097152` | Gibt an, ob die Textrichtungs‑Eigenschaft geändert wurde. |
| RelativeIndent | `128` | Gibt an, ob die relative Einzugs‑Eigenschaft für den Stil geändert wurde. Nur für dynamische Stile, wie bedingte Formatierung. |
| AlignmentSettings | `4161664` | Gibt an, ob eine oder mehrere ausrichtungsbezogene Eigenschaften (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) geändert wurden. |
| Pattern | `4194304` | Gibt an, ob das Muster der Schattierung geändert wurde. |
| ForegroundColor | `8388608` | Gibt an, ob die Vordergrundfarbe geändert wurde. |
| BackgroundColor | `16777216` | Gibt an, ob die Hintergrundfarbe geändert wurde. |
| CellShading | `29360128` | Gibt an, ob eine oder mehrere schattierungsbezogene Eigenschaften (Pattern, ForegroundColor, BackgroundColor) geändert wurden. |
| Locked | `67108864` | Gibt an, ob die gesperrte Eigenschaft geändert wurde. |
| HideFormula | `134217728` | Gibt an, ob das Ausblenden der Formel geändert wurde. |
| ProtectionSettings | `201326592` | Gibt an, ob eine oder mehrere schutzbezogene Eigenschaften (Locked, HideFormula) geändert wurden. |
| FontSize | `1` | Gibt an, ob die Schriftgröße geändert wurde. |
| FontName | `2` | Gibt an, ob der Schriftname geändert wurde. |
| FontColor | `3` | Gibt an, ob die Schriftfarbe geändert wurde. |
| FontWeight | `4` | Gibt an, ob die Schriftstärke geändert wurde. |
| FontItalic | `5` | Gibt an, ob die kursive Eigenschaft der Schrift geändert wurde. |
| FontUnderline | `6` | Gibt an, ob die Unterstreichungs‑Eigenschaft der Schrift geändert wurde. |
| FontStrike | `7` | Gibt an, ob die Durchstreichungs‑Eigenschaft der Schrift geändert wurde. |
| FontScript | `8` | Gibt an, ob die Tief- oder Hochstellungseigenschaft der Schrift geändert wurde. |
| FontFamily | `9` | Gibt an, ob die Schriftfamilie geändert wurde. |
| FontCharset | `10` | Gibt an, ob der Zeichensatz der Schrift geändert wurde. |
| FontScheme | `11` | nicht verwendet. |
| FontDirty | `12` | nicht verwendet. |
| FontSpellingError | `13` | nicht verwendet. |
| FontUFillTx | `14` | nicht verwendet. |
| FontSpacing | `15` | nicht verwendet. |
| FontKerning | `16` | nicht verwendet. |
| FontEqualize | `17` | nicht verwendet. |
| FontCap | `18` | nicht verwendet. |
| FontVerticalText | `19` |  |
| Font | `31` | Gibt an, ob eine oder mehrere Eigenschaften für die Schrift des Stils geändert wurden. |
| All | `234881023` | Alle Eigenschaften, die für den Stil geändert werden können. |
| None | `0` | Es wurde keine Eigenschaft angegeben. |

### Hinweise

Kombinationen mehrerer Eigenschaften werden zur Benutzerfreundlichkeit definiert. Beim Prüfen, ob sie für einen Stil geändert wurden, gibt der zurückgegebene Wert an, ob eine oder mehrere Eigenschaften in der Kombination geändert wurden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Setzen Sie einige Werte im Arbeitsblatt
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Erstelle einen neuen Stil
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].SetStyle(style);

            // Überprüfe, welche Stileigenschaften geändert wurden
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Ergebnisse ausgeben
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


