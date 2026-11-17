---
title: "Enum StyleModifyFlag"
linktitle: "StyleModifyFlag"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enum StyleModifyFlag. Encapsula el objeto que representa stylemodifyflag en Go."
type: docs
weight: 200
url: /es/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

The style modified flags.

```go

type StyleModifyFlag int32


```

## Fields

| Field | Description |
| --- | --- |
| [LeftBorder](./leftborder/) | Indica si el borde izquierdo ha sido modificado para el estilo. |
| [RightBorder](./rightborder/) | Indica si el borde derecho ha sido modificado para el estilo. |
| [TopBorder](./topborder/) | Indica si el borde superior ha sido modificado para el estilo. |
| [BottomBorder](./bottomborder/) | Indica si el borde inferior ha sido modificado para el estilo. |
| [DiagonalDownBorder](./diagonaldownborder/) | Indica si el borde diagonal descendente ha sido modificado para el estilo. |
| [DiagonalUpBorder](./diagonalupborder/) | Indica si el borde diagonal ascendente ha sido modificado para el estilo. |
| [HorizontalBorder](./horizontalborder/) | Indica si el borde horizontal ha sido modificado para el estilo. Solo para estilos dinámicos, como el formato condicional. |
| [VerticalBorder](./verticalborder/) | Indica si el borde vertical ha sido modificado para el estilo. Solo para estilos dinámicos, como el formato condicional. |
| [SideBorders](./sideborders/) | Indicates the four side borders: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> and <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Indica los bordes diagonales: <see cref="DiagonalDownBorder"/> y <see cref="DiagonalUpBorder"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Indica los bordes del estilo dinámico: <see cref="HorizontalBorder"/> y <see cref="VerticalBorder"/>. |
| [Borders](./borders/) | Indica si uno o más bordes (<see cref="LeftBorder"/>, <see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>, <see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>) han sido modificados para el estilo. |
| [NumberFormat](./numberformat/) | Indica si el formato numérico ha sido modificado. |
| [HorizontalAlignment](./horizontalalignment/) | Indica si la alineación horizontal ha sido modificada. |
| [VerticalAlignment](./verticalalignment/) | Indica si la alineación vertical ha sido modificada. |
| [Indent](./indent/) | Indica si la propiedad de sangría ha sido modificada. |
| [Rotation](./rotation/) | Indica si la propiedad de rotación ha sido modificada. |
| [WrapText](./wraptext/) | Indica si la propiedad de ajuste de texto ha sido modificada. |
| [ShrinkToFit](./shrinktofit/) | Indica si la propiedad de encoger para ajustar ha sido modificada. |
| [TextDirection](./textdirection/) | Indica si la propiedad de dirección del texto ha sido modificada. |
| [RelativeIndent](./relativeindent/) | Indica si la propiedad de sangría relativa ha sido modificada para el estilo. Solo para estilo dinámico, como el formato condicional. |
| [AlignmentSettings](./alignmentsettings/) | Indica si una o más propiedades relacionadas con la alineación (<see cref="HorizontalAlignment"/>,<see cref="VerticalAlignment"/>, <see cref="Rotation"/>, <see cref="WrapText"/>,<see cref="WrapText"/>, <see cref="Indent"/>, <see cref="ShrinkToFit"/>, <see cref="TextDirection"/>,<see cref="RelativeIndent"/>) han sido modificadas. |
| [Pattern](./pattern/) | Indica si el patrón del sombreado ha sido modificado. |
| [ForegroundColor](./foregroundcolor/) | Indica si el color de primer plano ha sido modificado. |
| [BackgroundColor](./backgroundcolor/) | Indica si el color de fondo ha sido modificado. |
| [CellShading](./cellshading/) | Indica si una o más propiedades relacionadas con el sombreado (<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>) han sido modificadas. |
| [Locked](./locked/) | Indica si la propiedad de bloqueo ha sido modificada. |
| [HideFormula](./hideformula/) | Indica si la propiedad de ocultar fórmula ha sido modificada. |
| [ProtectionSettings](./protectionsettings/) | Indica si una o más propiedades relacionadas con la protección (<see cref="Locked"/>,<see cref="HideFormula"/>) han sido modificadas. |
| [FontSize](./fontsize/) | Indica si el tamaño de fuente ha sido modificado. |
| [FontName](./fontname/) | Indica si el nombre de fuente ha sido modificado. |
| [FontColor](./fontcolor/) | Indica si el color de fuente ha sido modificado. |
| [FontWeight](./fontweight/) | Indica si el grosor de fuente ha sido modificado. |
| [FontItalic](./fontitalic/) | Indica si la propiedad cursiva de la fuente ha sido modificada. |
| [FontUnderline](./fontunderline/) | Indica si la propiedad subrayado de la fuente ha sido modificada. |
| [FontStrike](./fontstrike/) | Indica si la propiedad de tachado de la fuente ha sido modificada. |
| [FontScript](./fontscript/) | Indica si la propiedad de subíndice o superíndice de la fuente ha sido modificada. |
| [FontFamily](./fontfamily/) | Indica si la familia de fuentes ha sido modificada. |
| [FontCharset](./fontcharset/) | Indica si el conjunto de caracteres de la fuente ha sido modificado. |
| [FontScheme](./fontscheme/) | no utilizado. |
| [FontDirty](./fontdirty/) | no utilizado. |
| [FontSpellingError](./fontspellingerror/) | no utilizado. |
| [FontUFillTx](./fontufilltx/) | no utilizado. |
| [FontSpacing](./fontspacing/) | no utilizado. |
| [FontKerning](./fontkerning/) | no utilizado. |
| [FontEqualize](./fontequalize/) | no utilizado. |
| [FontCap](./fontcap/) | no utilizado. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Indica si una o más propiedades han sido modificadas para la fuente del estilo. |
| [All](./all/) | Todas las propiedades que pueden ser modificadas para el estilo. |
| [None](./none/) | No se ha especificado ninguna propiedad. |
