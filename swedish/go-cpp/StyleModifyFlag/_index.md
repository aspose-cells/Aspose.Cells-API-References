---
title: "StyleModifyFlag Enum"
linktitle: "StyleModifyFlag"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "StyleModifyFlag enum. Inkapslar objektet som representerar stylemodifyflag i Go."
type: docs
weight: 200
url: /sv/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

Stilens modifieringsflaggor.

```go

type StyleModifyFlag int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [LeftBorder](./leftborder/) | Indikerar om vänster kant har ändrats för stilen. |
| [RightBorder](./rightborder/) | Indikerar om höger kant har ändrats för stilen. |
| [TopBorder](./topborder/) | Indikerar om den övre kanten har ändrats för stilen. |
| [BottomBorder](./bottomborder/) | Indikerar om den nedre kanten har ändrats för stilen. |
| [DiagonalDownBorder](./diagonaldownborder/) | Indikerar om den diagonala nedåtkanten har ändrats för stilen. |
| [DiagonalUpBorder](./diagonalupborder/) | Indikerar om den diagonala uppåtkanten har ändrats för stilen. |
| [HorizontalBorder](./horizontalborder/) | Indikerar om den horisontella kanten har ändrats för stilen. Endast för dynamisk stil, till exempel villkorsstyrd formatering. |
| [VerticalBorder](./verticalborder/) | Indikerar om den vertikala kanten har ändrats för stilen. Endast för dynamisk stil, till exempel villkorsstyrd formatering. |
| [SideBorders](./sideborders/) | Anger de fyra sidokanterna: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> och <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Indikerar diagonala kanter: <see cref="DiagonalDownBorder"/> och <see cref="DiagonalUpBorder"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Indikerar kanter för dynamisk stil: <see cref="HorizontalBorder"/> och <see cref="VerticalBorder"/>. |
| [Borders](./borders/) | Indikerar om en eller flera kanter(<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>,<see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>) har ändrats för stilen. |
| [NumberFormat](./numberformat/) | Indikerar om talformat har ändrats. |
| [HorizontalAlignment](./horizontalalignment/) | Indikerar om horisontell justering har ändrats. |
| [VerticalAlignment](./verticalalignment/) | Indikerar om vertikal justering har ändrats. |
| [Indent](./indent/) | Indikerar om indragsegenskap har ändrats. |
| [Rotation](./rotation/) | Indikerar om rotationsegenskap har ändrats. |
| [WrapText](./wraptext/) | Indikerar om egenskapen för radbrytning har ändrats. |
| [ShrinkToFit](./shrinktofit/) | Indikerar om egenskapen för krympning för att passa har ändrats. |
| [TextDirection](./textdirection/) | Indikerar om egenskapen för textriktning har ändrats. |
| [RelativeIndent](./relativeindent/) | Indikerar om relativ indragsegenskap har ändrats för stilen. Endast för dynamisk stil, till exempel villkorsstyrd formatering. |
| [AlignmentSettings](./alignmentsettings/) | Indikerar om en eller flera justeringsrelaterade egenskaper(<see cref="HorizontalAlignment"/>,<see cref="VerticalAlignment"/>, <see cref="Rotation"/>, <see cref="WrapText"/>,<see cref="WrapText"/>, <see cref="Indent"/>, <see cref="ShrinkToFit"/>, <see cref="TextDirection"/>,<see cref="RelativeIndent"/>) har ändrats. |
| [Pattern](./pattern/) | Indikerar om mönstret för skuggning har ändrats. |
| [ForegroundColor](./foregroundcolor/) | Indikerar om förgrundsfärg har ändrats. |
| [BackgroundColor](./backgroundcolor/) | Indikerar om bakgrundsfärg har ändrats. |
| [CellShading](./cellshading/) | Indikerar om en eller flera skuggningsrelaterade egenskaper(<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>) har ändrats. |
| [Locked](./locked/) | Indikerar om låst egenskap har ändrats. |
| [HideFormula](./hideformula/) | Indikerar om dölja formel har ändrats. |
| [ProtectionSettings](./protectionsettings/) | Anger om en eller flera skyddrelaterade egenskaper(<see cref=\"Locked\"/>,<see cref=\"HideFormula\"/>) har ändrats. |
| [FontSize](./fontsize/) | Anger om teckenstorlek har ändrats. |
| [FontName](./fontname/) | Anger om teckensnittets namn har ändrats. |
| [FontColor](./fontcolor/) | Anger om teckenfärg har ändrats. |
| [FontWeight](./fontweight/) | Anger om teckenvikt har ändrats. |
| [FontItalic](./fontitalic/) | Anger om kursiv‑egenskapen för teckensnittet har ändrats. |
| [FontUnderline](./fontunderline/) | Anger om understrykningsegenskapen för teckensnittet har ändrats. |
| [FontStrike](./fontstrike/) | Anger om genomstrykningsegenskapen för teckensnittet har ändrats. |
| [FontScript](./fontscript/) | Anger om nedsänkt eller upphöjd egenskap för teckensnittet har ändrats. |
| [FontFamily](./fontfamily/) | Anger om teckensnittsfamilj har ändrats. |
| [FontCharset](./fontcharset/) | Anger om teckensnittets teckenuppsättning har ändrats. |
| [FontScheme](./fontscheme/) | oanvänd. |
| [FontDirty](./fontdirty/) | oanvänd. |
| [FontSpellingError](./fontspellingerror/) | oanvänd. |
| [FontUFillTx](./fontufilltx/) | oanvänd. |
| [FontSpacing](./fontspacing/) | oanvänd. |
| [FontKerning](./fontkerning/) | oanvänd. |
| [FontEqualize](./fontequalize/) | oanvänd. |
| [FontCap](./fontcap/) | oanvänd. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Anger om en eller flera egenskaper har ändrats för stilens teckensnitt. |
| [All](./all/) | Alla egenskaper som kan ändras för stilen. |
| [None](./none/) | Ingen egenskap har angivits. |
