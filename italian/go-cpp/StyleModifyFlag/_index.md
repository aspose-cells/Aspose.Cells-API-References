---
title: "Enum StyleModifyFlag"
linktitle: "StyleModifyFlag"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum StyleModifyFlag. Incapsula l'oggetto che rappresenta stylemodifyflag in Go."
type: docs
weight: 200
url: /it/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

I flag di stile modificati.

```go

type StyleModifyFlag int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [LeftBorder](./leftborder/) | Indica se il bordo sinistro è stato modificato per lo stile. |
| [RightBorder](./rightborder/) | Indica se il bordo destro è stato modificato per lo stile. |
| [TopBorder](./topborder/) | Indica se il bordo superiore è stato modificato per lo stile. |
| [BottomBorder](./bottomborder/) | Indica se il bordo inferiore è stato modificato per lo stile. |
| [DiagonalDownBorder](./diagonaldownborder/) | Indica se il bordo diagonale verso il basso è stato modificato per lo stile. |
| [DiagonalUpBorder](./diagonalupborder/) | Indica se il bordo diagonale verso l'alto è stato modificato per lo stile. |
| [HorizontalBorder](./horizontalborder/) | Indica se il bordo orizzontale è stato modificato per lo stile. Solo per stile dinamico, come la formattazione condizionale. |
| [VerticalBorder](./verticalborder/) | Indica se il bordo verticale è stato modificato per lo stile. Solo per stile dinamico, come la formattazione condizionale. |
| [SideBorders](./sideborders/) | Indica i quattro bordi laterali: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> e <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Indica i bordi diagonali: <see cref="DiagonalDownBorder"/> e <see cref="DiagonalUpBorder"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Indica i bordi dello stile dinamico: <see cref="HorizontalBorder"/> e <see cref="VerticalBorder"/>. |
| [Borders](./borders/) | Indica se uno o più bordi (<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>,<see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>) sono stati modificati per lo stile. |
| [NumberFormat](./numberformat/) | Indica se il formato numerico è stato modificato. |
| [HorizontalAlignment](./horizontalalignment/) | Indica se l'allineamento orizzontale è stato modificato. |
| [VerticalAlignment](./verticalalignment/) | Indica se l'allineamento verticale è stato modificato. |
| [Indent](./indent/) | Indica se la proprietà di rientro è stata modificata. |
| [Rotation](./rotation/) | Indica se la proprietà di rotazione è stata modificata. |
| [WrapText](./wraptext/) | Indica se la proprietà di testo a capo è stata modificata. |
| [ShrinkToFit](./shrinktofit/) | Indica se la proprietà di riduzione per adattamento è stata modificata. |
| [TextDirection](./textdirection/) | Indica se la proprietà di direzione del testo è stata modificata. |
| [RelativeIndent](./relativeindent/) | Indica se la proprietà di rientro relativo è stata modificata per lo stile. Solo per stile dinamico, come la formattazione condizionale. |
| [AlignmentSettings](./alignmentsettings/) | Indica se una o più proprietà relative all'allineamento (<see cref=\"HorizontalAlignment\"/>,<see cref=\"VerticalAlignment\"/>, <see cref=\"Rotation\"/>, <see cref=\"WrapText\"/>,<see cref=\"WrapText\"/>, <see cref=\"Indent\"/>, <see cref=\"ShrinkToFit\"/>, <see cref=\"TextDirection\"/>,<see cref=\"RelativeIndent\"/>) sono state modificate. |
| [Pattern](./pattern/) | Indica se il modello dell'ombreggiatura è stato modificato. |
| [ForegroundColor](./foregroundcolor/) | Indica se il colore di primo piano è stato modificato. |
| [BackgroundColor](./backgroundcolor/) | Indica se il colore di sfondo è stato modificato. |
| [CellShading](./cellshading/) | Indica se una o più proprietà relative all'ombreggiatura (<see cref=\"Pattern\"/>,<see cref=\"ForegroundColor\"/>, <see cref=\"BackgroundColor\"/>) sono state modificate. |
| [Locked](./locked/) | Indica se la proprietà bloccata è stata modificata. |
| [HideFormula](./hideformula/) | Indica se la proprietà nascondi formula è stata modificata. |
| [ProtectionSettings](./protectionsettings/) | Indica se una o più proprietà relative alla protezione (<see cref=\"Locked\"/>,<see cref=\"HideFormula\"/>) sono state modificate. |
| [FontSize](./fontsize/) | Indica se la dimensione del carattere è stata modificata. |
| [FontName](./fontname/) | Indica se il nome del carattere è stato modificato. |
| [FontColor](./fontcolor/) | Indica se il colore del carattere è stato modificato. |
| [FontWeight](./fontweight/) | Indica se lo spessore del carattere è stato modificato. |
| [FontItalic](./fontitalic/) | Indica se la proprietà corsivo del carattere è stata modificata. |
| [FontUnderline](./fontunderline/) | Indica se la proprietà sottolineato del carattere è stata modificata. |
| [FontStrike](./fontstrike/) | Indica se la proprietà barrato del carattere è stata modificata. |
| [FontScript](./fontscript/) | Indica se la proprietà apice o pedice del carattere è stata modificata. |
| [FontFamily](./fontfamily/) | Indica se la famiglia del carattere è stata modificata. |
| [FontCharset](./fontcharset/) | Indica se il set di caratteri del font è stato modificato. |
| [FontScheme](./fontscheme/) | non utilizzato. |
| [FontDirty](./fontdirty/) | non utilizzato. |
| [FontSpellingError](./fontspellingerror/) | non utilizzato. |
| [FontUFillTx](./fontufilltx/) | non utilizzato. |
| [FontSpacing](./fontspacing/) | non utilizzato. |
| [FontKerning](./fontkerning/) | non utilizzato. |
| [FontEqualize](./fontequalize/) | non utilizzato. |
| [FontCap](./fontcap/) | non utilizzato. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Indica se una o più proprietà sono state modificate per il font dello stile. |
| [All](./all/) | Tutte le proprietà che possono essere modificate per lo stile. |
| [None](./none/) | Nessuna proprietà è stata specificata. |
