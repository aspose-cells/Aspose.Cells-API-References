---
title: "StyleModifyFlag Enum"
linktitle: "StyleModifyFlag"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "StyleModifyFlag enum. Encapsule l'objet qui représente stylemodifyflag en Go."
type: docs
weight: 200
url: /fr/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

Les indicateurs de style modifié.

```go

type StyleModifyFlag int32


```

## Champs

| Champ | Description |
| --- | --- |
| [LeftBorder](./leftborder/) | Indique si la bordure gauche a été modifiée pour le style. |
| [RightBorder](./rightborder/) | Indique si la bordure droite a été modifiée pour le style. |
| [TopBorder](./topborder/) | Indique si la bordure supérieure a été modifiée pour le style. |
| [BottomBorder](./bottomborder/) | Indique si la bordure inférieure a été modifiée pour le style. |
| [DiagonalDownBorder](./diagonaldownborder/) | Indique si la bordure diagonale descendante a été modifiée pour le style. |
| [DiagonalUpBorder](./diagonalupborder/) | Indique si la bordure diagonale ascendante a été modifiée pour le style. |
| [HorizontalBorder](./horizontalborder/) | Indique si la bordure horizontale a été modifiée pour le style. Seulement pour les styles dynamiques, tels que le formatage conditionnel. |
| [VerticalBorder](./verticalborder/) | Indique si la bordure verticale a été modifiée pour le style. Seulement pour les styles dynamiques, tels que le formatage conditionnel. |
| [SideBorders](./sideborders/) | Indique les bordures des quatre côtés : <see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/> et <see cref=\"BottomBorder\"/>. |
| [Diagonal](./diagonal/) | Indique les bordures diagonales : <see cref="DiagonalDownBorder"/> et <see cref="DiagonalUpBorder"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Indique les bordures du style dynamique : <see cref="HorizontalBorder"/> et <see cref="VerticalBorder"/>. |
| [Borders](./borders/) | Indique si une ou plusieurs bordures(<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>,<see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>) ont été modifiées pour le style. |
| [NumberFormat](./numberformat/) | Indique si le format numérique a été modifié. |
| [HorizontalAlignment](./horizontalalignment/) | Indique si l'alignement horizontal a été modifié. |
| [VerticalAlignment](./verticalalignment/) | Indique si l'alignement vertical a été modifié. |
| [Indent](./indent/) | Indique si la propriété d'indentation a été modifiée. |
| [Rotation](./rotation/) | Indique si la propriété de rotation a été modifiée. |
| [WrapText](./wraptext/) | Indique si la propriété de retour à la ligne du texte a été modifiée. |
| [ShrinkToFit](./shrinktofit/) | Indique si la propriété de réduction pour ajuster a été modifiée. |
| [TextDirection](./textdirection/) | Indique si la propriété de direction du texte a été modifiée. |
| [RelativeIndent](./relativeindent/) | Indique si la propriété d'indentation relative a été modifiée pour le style. Seulement pour le style dynamique, tel que le formatage conditionnel. |
| [AlignmentSettings](./alignmentsettings/) | Indique si une ou plusieurs propriétés liées à l'alignement (<see cref=\"HorizontalAlignment\"/>,<see cref=\"VerticalAlignment\"/>, <see cref=\"Rotation\"/>, <see cref=\"WrapText\"/>,<see cref=\"WrapText\"/>, <see cref=\"Indent\"/>, <see cref=\"ShrinkToFit\"/>, <see cref=\"TextDirection\"/>,<see cref=\"RelativeIndent\"/>) ont été modifiées. |
| [Pattern](./pattern/) | Indique si le motif de l'ombrage a été modifié. |
| [ForegroundColor](./foregroundcolor/) | Indique si la couleur de premier plan a été modifiée. |
| [BackgroundColor](./backgroundcolor/) | Indique si la couleur d'arrière-plan a été modifiée. |
| [CellShading](./cellshading/) | Indique si une ou plusieurs propriétés liées à l'ombrage (<see cref=\"Pattern\"/>,<see cref=\"ForegroundColor\"/>, <see cref=\"BackgroundColor\"/>) ont été modifiées. |
| [Locked](./locked/) | Indique si la propriété verrouillée a été modifiée. |
| [HideFormula](./hideformula/) | Indique si le masquage de la formule a été modifié. |
| [ProtectionSettings](./protectionsettings/) | Indique si une ou plusieurs propriétés liées à la protection (<see cref=\"Locked\"/>,<see cref=\"HideFormula\"/>) ont été modifiées. |
| [FontSize](./fontsize/) | Indique si la taille de la police a été modifiée. |
| [FontName](./fontname/) | Indique si le nom de la police a été modifié. |
| [FontColor](./fontcolor/) | Indique si la couleur de la police a été modifiée. |
| [FontWeight](./fontweight/) | Indique si le poids de la police a été modifié. |
| [FontItalic](./fontitalic/) | Indique si la propriété italique de la police a été modifiée. |
| [FontUnderline](./fontunderline/) | Indique si la propriété soulignée de la police a été modifiée. |
| [FontStrike](./fontstrike/) | Indique si la propriété de texte barré de la police a été modifiée. |
| [FontScript](./fontscript/) | Indique si la propriété indice ou exposant de la police a été modifiée. |
| [FontFamily](./fontfamily/) | Indique si la famille de police a été modifiée. |
| [FontCharset](./fontcharset/) | Indique si le jeu de caractères de la police a été modifié. |
| [FontScheme](./fontscheme/) | non utilisé. |
| [FontDirty](./fontdirty/) | non utilisé. |
| [FontSpellingError](./fontspellingerror/) | non utilisé. |
| [FontUFillTx](./fontufilltx/) | non utilisé. |
| [FontSpacing](./fontspacing/) | non utilisé. |
| [FontKerning](./fontkerning/) | non utilisé. |
| [FontEqualize](./fontequalize/) | non utilisé. |
| [FontCap](./fontcap/) | non utilisé. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Indique si une ou plusieurs propriétés ont été modifiées pour la police du style. |
| [All](./all/) | Toutes les propriétés pouvant être modifiées pour le style. |
| [None](./none/) | Aucune propriété n'a été spécifiée. |
