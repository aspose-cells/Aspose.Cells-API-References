---
title: "StyleModifyFlag 枚举"
linktitle: "StyleModifyFlag"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "StyleModifyFlag 枚举。封装在 Go 中表示 stylemodifyflag 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

样式修改标志。

```go

type StyleModifyFlag int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [LeftBorder](./leftborder/) | 指示样式的左边框是否已修改。 |
| [RightBorder](./rightborder/) | 指示样式的右边框是否已修改。 |
| [TopBorder](./topborder/) | 指示样式的上边框是否已修改。 |
| [BottomBorder](./bottomborder/) | 指示样式的下边框是否已修改。 |
| [DiagonalDownBorder](./diagonaldownborder/) | 指示样式的向下对角线边框是否已修改。 |
| [DiagonalUpBorder](./diagonalupborder/) | 指示样式的向上对角线边框是否已修改。 |
| [HorizontalBorder](./horizontalborder/) | 指示样式的水平边框是否已修改。仅适用于动态样式，例如条件格式化。 |
| [VerticalBorder](./verticalborder/) | 指示样式的垂直边框是否已修改。仅适用于动态样式，例如条件格式化。 |
| [SideBorders](./sideborders/) | 指示四个侧边框：<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> 和 <see cref="BottomBorder"/>。 |
| [Diagonal](./diagonal/) | 指示对角线边框：<see cref="DiagonalDownBorder"/> 和 <see cref="DiagonalUpBorder"/>。 |
| [DynamicStyleBorders](./dynamicstyleborders/) | 指示动态样式的边框：<see cref="HorizontalBorder"/> 和 <see cref="VerticalBorder"/>。 |
| [Borders](./borders/) | 指示样式是否已修改一个或多个边框（<see cref="LeftBorder"/>、<see cref="RightBorder"/>、<see cref="TopBorder"/>、<see cref="BottomBorder"/>、<see cref="Diagonal"/>、<see cref="HorizontalBorder"/>、<see cref="VerticalBorder"/>）。 |
| [NumberFormat](./numberformat/) | 指示 numberformat 是否已修改。 |
| [HorizontalAlignment](./horizontalalignment/) | 指示水平对齐是否已被修改。 |
| [VerticalAlignment](./verticalalignment/) | 指示垂直对齐是否已被修改。 |
| [Indent](./indent/) | 指示缩进属性是否已被修改。 |
| [Rotation](./rotation/) | 指示旋转属性是否已被修改。 |
| [WrapText](./wraptext/) | 指示自动换行属性是否已被修改。 |
| [ShrinkToFit](./shrinktofit/) | 指示缩小以适应属性是否已被修改。 |
| [TextDirection](./textdirection/) | 指示文本方向属性是否已被修改。 |
| [RelativeIndent](./relativeindent/) | 指示相对缩进属性在样式中是否已被修改。仅适用于动态样式，例如条件格式化。 |
| [AlignmentSettings](./alignmentsettings/) | 指示一个或多个对齐相关属性（<see cref="HorizontalAlignment"/>,<see cref="VerticalAlignment"/>, <see cref="Rotation"/>, <see cref="WrapText"/>,<see cref="WrapText"/>, <see cref="Indent"/>, <see cref="ShrinkToFit"/>, <see cref="TextDirection"/>,<see cref="RelativeIndent"/>)是否已被修改。 |
| [Pattern](./pattern/) | 指示阴影的图案是否已被修改。 |
| [ForegroundColor](./foregroundcolor/) | 指示前景色是否已被修改。 |
| [BackgroundColor](./backgroundcolor/) | 指示背景色是否已被修改。 |
| [CellShading](./cellshading/) | 指示一个或多个阴影相关属性（<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>)是否已被修改。 |
| [Locked](./locked/) | 指示锁定属性是否已被修改。 |
| [HideFormula](./hideformula/) | 指示隐藏公式是否已被修改。 |
| [ProtectionSettings](./protectionsettings/) | 指示一个或多个保护相关属性（<see cref="Locked"/>,<see cref="HideFormula"/>)是否已被修改。 |
| [FontSize](./fontsize/) | 指示字体大小是否已被修改。 |
| [FontName](./fontname/) | 指示字体名称是否已被修改。 |
| [FontColor](./fontcolor/) | 指示字体颜色是否已被修改。 |
| [FontWeight](./fontweight/) | 指示字体粗细是否已被修改。 |
| [FontItalic](./fontitalic/) | 指示字体的斜体属性是否已被修改。 |
| [FontUnderline](./fontunderline/) | 指示字体的下划线属性是否已被修改。 |
| [FontStrike](./fontstrike/) | 指示字体的删除线属性是否已被修改。 |
| [FontScript](./fontscript/) | 指示字体的下标或上标属性是否已被修改。 |
| [FontFamily](./fontfamily/) | 指示字体族是否已被修改。 |
| [FontCharset](./fontcharset/) | 指示字体的字符集是否已被修改。 |
| [FontScheme](./fontscheme/) | 未使用。 |
| [FontDirty](./fontdirty/) | 未使用。 |
| [FontSpellingError](./fontspellingerror/) | 未使用。 |
| [FontUFillTx](./fontufilltx/) | 未使用。 |
| [FontSpacing](./fontspacing/) | 未使用。 |
| [FontKerning](./fontkerning/) | 未使用。 |
| [FontEqualize](./fontequalize/) | 未使用。 |
| [FontCap](./fontcap/) | 未使用。 |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | 指示样式的字体是否已修改一个或多个属性。 |
| [All](./all/) | 可用于样式的所有可修改属性。 |
| [None](./none/) | 未指定任何属性。 |
