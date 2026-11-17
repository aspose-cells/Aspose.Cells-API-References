---
title: "Перечисление StyleModifyFlag"
linktitle: "StyleModifyFlag"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление StyleModifyFlag. Инкапсулирует объект, представляющий stylemodifyflag в Go."
type: docs
weight: 200
url: /ru/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

Флаги изменённого стиля.

```go

type StyleModifyFlag int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [LeftBorder](./leftborder/) | Указывает, изменена ли левая граница стиля. |
| [RightBorder](./rightborder/) | Указывает, изменена ли правая граница стиля. |
| [TopBorder](./topborder/) | Указывает, изменена ли верхняя граница стиля. |
| [BottomBorder](./bottomborder/) | Указывает, изменена ли нижняя граница стиля. |
| [DiagonalDownBorder](./diagonaldownborder/) | Указывает, изменена ли диагональная граница вниз у стиля. |
| [DiagonalUpBorder](./diagonalupborder/) | Указывает, изменена ли диагональная граница вверх у стиля. |
| [HorizontalBorder](./horizontalborder/) | Указывает, изменена ли горизонтальная граница у стиля. Только для динамического стиля, например условного форматирования. |
| [VerticalBorder](./verticalborder/) | Указывает, изменена ли вертикальная граница у стиля. Только для динамического стиля, например условного форматирования. |
| [SideBorders](./sideborders/) | Указывает четыре боковые границы: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> и <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Указывает диагональные границы: <see cref=\"DiagonalDownBorder\"/> и <see cref=\"DiagonalUpBorder\"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Указывает границы динамического стиля: <see cref=\"HorizontalBorder\"/> и <see cref=\"VerticalBorder\"/>. |
| [Borders](./borders/) | Указывает, изменена ли одна или несколько границ (<see cref=\"LeftBorder\"/>, <see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/>, <see cref=\"BottomBorder\"/>, <see cref=\"Diagonal\"/>, <see cref=\"HorizontalBorder\"/>, <see cref=\"VerticalBorder\"/>) у стиля. |
| [NumberFormat](./numberformat/) | Указывает, изменён ли формат числа. |
| [HorizontalAlignment](./horizontalalignment/) | Указывает, было ли изменено горизонтальное выравнивание. |
| [VerticalAlignment](./verticalalignment/) | Указывает, было ли изменено вертикальное выравнивание. |
| [Indent](./indent/) | Указывает, было ли изменено свойство отступа. |
| [Rotation](./rotation/) | Указывает, было ли изменено свойство вращения. |
| [WrapText](./wraptext/) | Указывает, было ли изменено свойство переноса текста. |
| [ShrinkToFit](./shrinktofit/) | Указывает, было ли изменено свойство сжатия до размеров. |
| [TextDirection](./textdirection/) | Указывает, было ли изменено свойство направления текста. |
| [RelativeIndent](./relativeindent/) | Указывает, было ли изменено свойство относительного отступа для стиля. Только для динамического стиля, например условного форматирования. |
| [AlignmentSettings](./alignmentsettings/) | Указывает, было ли изменено одно или несколько свойств, связанных с выравниванием (<see cref=\"HorizontalAlignment\"/>,<see cref=\"VerticalAlignment\"/>, <see cref=\"Rotation\"/>, <see cref=\"WrapText\"/>,<see cref=\"WrapText\"/>, <see cref=\"Indent\"/>, <see cref=\"ShrinkToFit\"/>, <see cref=\"TextDirection\"/>,<see cref=\"RelativeIndent\"/>) . |
| [Pattern](./pattern/) | Указывает, был ли изменён шаблон затенения. |
| [ForegroundColor](./foregroundcolor/) | Указывает, был ли изменён цвет переднего плана. |
| [BackgroundColor](./backgroundcolor/) | Указывает, был ли изменён цвет фона. |
| [CellShading](./cellshading/) | Указывает, было ли изменено одно или несколько свойств, связанных с затенением (<see cref=\"Pattern\"/>,<see cref=\"ForegroundColor\"/>, <see cref=\"BackgroundColor\"/>) . |
| [Locked](./locked/) | Указывает, было ли изменено свойство блокировки. |
| [HideFormula](./hideformula/) | Указывает, было ли изменено свойство скрытия формулы. |
| [ProtectionSettings](./protectionsettings/) | Указывает, было ли изменено одно или несколько свойств, связанных с защитой (<see cref=\"Locked\"/>,<see cref=\"HideFormula\"/>) . |
| [FontSize](./fontsize/) | Указывает, был ли изменён размер шрифта. |
| [FontName](./fontname/) | Указывает, было ли изменено имя шрифта. |
| [FontColor](./fontcolor/) | Указывает, был ли изменён цвет шрифта. |
| [FontWeight](./fontweight/) | Указывает, был ли изменён вес шрифта. |
| [FontItalic](./fontitalic/) | Указывает, было ли изменено свойство курсивного начертания шрифта. |
| [FontUnderline](./fontunderline/) | Указывает, было ли изменено свойство подчёркивания шрифта. |
| [FontStrike](./fontstrike/) | Указывает, было ли изменено свойство зачеркивания шрифта. |
| [FontScript](./fontscript/) | Указывает, было ли изменено свойство нижнего или верхнего индекса шрифта. |
| [FontFamily](./fontfamily/) | Указывает, было ли изменено семейство шрифта. |
| [FontCharset](./fontcharset/) | Указывает, был ли изменён набор символов шрифта. |
| [FontScheme](./fontscheme/) | не используется. |
| [FontDirty](./fontdirty/) | не используется. |
| [FontSpellingError](./fontspellingerror/) | не используется. |
| [FontUFillTx](./fontufilltx/) | не используется. |
| [FontSpacing](./fontspacing/) | не используется. |
| [FontKerning](./fontkerning/) | не используется. |
| [FontEqualize](./fontequalize/) | не используется. |
| [FontCap](./fontcap/) | не используется. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Указывает, были ли изменены один или несколько свойств шрифта стиля. |
| [All](./all/) | Все свойства, которые могут быть изменены для стиля. |
| [None](./none/) | Свойство не указано. |
