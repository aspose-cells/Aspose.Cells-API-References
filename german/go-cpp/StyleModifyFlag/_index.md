---
title: "StyleModifyFlag Enum"
linktitle: "StyleModifyFlag"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "StyleModifyFlag enum. Kapselt das Objekt, das stylemodifyflag in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

Die vom Stil modifizierten Flags.

```go

type StyleModifyFlag int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [LeftBorder](./leftborder/) | Gibt an, ob der linke Rand für den Stil geändert wurde. |
| [RightBorder](./rightborder/) | Gibt an, ob der rechte Rand für den Stil geändert wurde. |
| [TopBorder](./topborder/) | Gibt an, ob der obere Rand für den Stil geändert wurde. |
| [BottomBorder](./bottomborder/) | Gibt an, ob der untere Rand für den Stil geändert wurde. |
| [DiagonalDownBorder](./diagonaldownborder/) | Gibt an, ob der diagonal-down Rand für den Stil geändert wurde. |
| [DiagonalUpBorder](./diagonalupborder/) | Gibt an, ob der diagonal-up Rand für den Stil geändert wurde. |
| [HorizontalBorder](./horizontalborder/) | Gibt an, ob der horizontale Rand für den Stil geändert wurde. Nur für dynamische Stile, wie z. B. bedingte Formatierung. |
| [VerticalBorder](./verticalborder/) | Gibt an, ob der vertikale Rand für den Stil geändert wurde. Nur für dynamische Stile, wie z. B. bedingte Formatierung. |
| [SideBorders](./sideborders/) | Gibt die vier Seitenränder an: <see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/> und <see cref=\"BottomBorder\"/>. |
| [Diagonal](./diagonal/) | Gibt diagonale Ränder an: <see cref=\"DiagonalDownBorder\"/> und <see cref=\"DiagonalUpBorder\"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Gibt Ränder des dynamischen Stils an: <see cref=\"HorizontalBorder\"/> und <see cref=\"VerticalBorder\"/>. |
| [Borders](./borders/) | Gibt an, ob ein oder mehrere Ränder(<see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/>, <see cref=\"BottomBorder\"/>,<see cref=\"Diagonal\"/>, <see cref=\"HorizontalBorder\"/>, <see cref=\"VerticalBorder\"/>) für den Stil geändert wurden. |
| [NumberFormat](./numberformat/) | Gibt an, ob das Zahlenformat geändert wurde. |
| [HorizontalAlignment](./horizontalalignment/) | Gibt an, ob die horizontale Ausrichtung geändert wurde. |
| [VerticalAlignment](./verticalalignment/) | Gibt an, ob die vertikale Ausrichtung geändert wurde. |
| [Indent](./indent/) | Gibt an, ob die Einzugseigenschaft geändert wurde. |
| [Rotation](./rotation/) | Gibt an, ob die Drehungseigenschaft geändert wurde. |
| [WrapText](./wraptext/) | Gibt an, ob die Zeilenumbruch‑Eigenschaft geändert wurde. |
| [ShrinkToFit](./shrinktofit/) | Gibt an, ob die 'Verkleinern, um anzupassen'-Eigenschaft geändert wurde. |
| [TextDirection](./textdirection/) | Gibt an, ob die Textrichtungseigenschaft geändert wurde. |
| [RelativeIndent](./relativeindent/) | Gibt an, ob die relative Einzugseigenschaft für den Stil geändert wurde. Nur für dynamische Stile, wie z. B. bedingte Formatierung. |
| [AlignmentSettings](./alignmentsettings/) | Gibt an, ob ein oder mehrere ausrichtungsbezogene Eigenschaften(<see cref=\"HorizontalAlignment\"/>,<see cref=\"VerticalAlignment\"/>, <see cref=\"Rotation\"/>, <see cref=\"WrapText\"/>,<see cref=\"WrapText\"/>, <see cref=\"Indent\"/>, <see cref=\"ShrinkToFit\"/>, <see cref=\"TextDirection\"/>,<see cref=\"RelativeIndent\"/>) geändert wurden. |
| [Pattern](./pattern/) | Gibt an, ob das Muster der Schattierung geändert wurde. |
| [ForegroundColor](./foregroundcolor/) | Gibt an, ob die Vordergrundfarbe geändert wurde. |
| [BackgroundColor](./backgroundcolor/) | Gibt an, ob die Hintergrundfarbe geändert wurde. |
| [CellShading](./cellshading/) | Gibt an, ob ein oder mehrere schattierungsbezogene Eigenschaften (<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>) geändert wurden. |
| [Locked](./locked/) | Gibt an, ob die gesperrte Eigenschaft geändert wurde. |
| [HideFormula](./hideformula/) | Gibt an, ob das Ausblenden der Formel geändert wurde. |
| [ProtectionSettings](./protectionsettings/) | Gibt an, ob ein oder mehrere schutzbezogene Eigenschaften (<see cref="Locked"/>,<see cref="HideFormula"/>) geändert wurden. |
| [FontSize](./fontsize/) | Gibt an, ob die Schriftgröße geändert wurde. |
| [FontName](./fontname/) | Gibt an, ob der Schriftname geändert wurde. |
| [FontColor](./fontcolor/) | Gibt an, ob die Schriftfarbe geändert wurde. |
| [FontWeight](./fontweight/) | Gibt an, ob die Schriftstärke geändert wurde. |
| [FontItalic](./fontitalic/) | Gibt an, ob die kursive Eigenschaft der Schrift geändert wurde. |
| [FontUnderline](./fontunderline/) | Gibt an, ob die Unterstreichungs‑Eigenschaft der Schrift geändert wurde. |
| [FontStrike](./fontstrike/) | Gibt an, ob die Durchstreich‑Eigenschaft der Schrift geändert wurde. |
| [FontScript](./fontscript/) | Gibt an, ob die Tief- oder Hochstellungseigenschaft der Schrift geändert wurde. |
| [FontFamily](./fontfamily/) | Gibt an, ob die Schriftfamilie geändert wurde. |
| [FontCharset](./fontcharset/) | Gibt an, ob der Zeichensatz der Schrift geändert wurde. |
| [FontScheme](./fontscheme/) | unbenutzt. |
| [FontDirty](./fontdirty/) | unbenutzt. |
| [FontSpellingError](./fontspellingerror/) | unbenutzt. |
| [FontUFillTx](./fontufilltx/) | unbenutzt. |
| [FontSpacing](./fontspacing/) | unbenutzt. |
| [FontKerning](./fontkerning/) | unbenutzt. |
| [FontEqualize](./fontequalize/) | unbenutzt. |
| [FontCap](./fontcap/) | unbenutzt. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Gibt an, ob ein oder mehrere Eigenschaften für die Schrift des Stils geändert wurden. |
| [All](./all/) | Alle Eigenschaften, die für den Stil geändert werden können. |
| [None](./none/) | Es wurde keine Eigenschaft angegeben. |
