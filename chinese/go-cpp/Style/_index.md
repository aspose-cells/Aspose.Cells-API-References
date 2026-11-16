---
title: "Style 类"
linktitle: "Style"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Style 类。封装表示 Go 中 style 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/style/
---

## Style class

表示 Excel 文档的显示样式，例如字体、颜色、对齐、边框等。Style 对象将所有样式属性（字体、数字格式、对齐方式等）作为属性包含。

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | 获取并设置背景主题颜色。 |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | 获取并设置背景主题颜色。 |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | 获取并设置前景主题颜色。 |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | 获取并设置前景主题颜色。 |
| [GetName](./getname/) | 获取或设置样式的名称。 |
| [SetName](./setname/) | 获取或设置样式的名称。 |
| [GetPattern](./getpattern/) | 获取或设置单元格背景图案类型。 |
| [SetPattern](./setpattern/) | 获取或设置单元格背景图案类型。 |
| [SetPatternColor](./setpatterncolor/) | 设置背景颜色。 |
| [GetBorders](./getborders/) | 获取样式的 BorderCollection。 |
| [GetBackgroundColor](./getbackgroundcolor/) | 获取或设置样式的背景颜色。 |
| [SetBackgroundColor](./setbackgroundcolor/) | 获取或设置样式的背景颜色。 |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | 获取并设置使用 32 位 ARGB 值的背景颜色。 |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | 获取并设置使用 32 位 ARGB 值的背景颜色。 |
| [GetForegroundColor](./getforegroundcolor/) | 获取或设置样式的前景颜色。 |
| [SetForegroundColor](./setforegroundcolor/) | 获取或设置样式的前景颜色。 |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | 获取并设置使用 32 位 ARGB 值的前景颜色。 |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | 获取并设置使用 32 位 ARGB 值的前景颜色。 |
| [Copy](./copy/) | 从另一个样式对象复制数据 |
| [GetHasBorders](./gethasborders/) | 检查是否已为该样式设置了边框。 |
| [GetParentStyle](./getparentstyle/) | 获取此样式的父样式。 |
| [Update](./update/) | 将命名样式应用于使用此命名样式的单元格的样式。它的作用相当于在完成样式修改后点击 "ok" 按钮。仅适用于命名样式。 |
| [IsNumberFormatApplied](./isnumberformatapplied/) | 指示是否应应用数字格式。 |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | 指示是否应应用数字格式。 |
| [IsFontApplied](./isfontapplied/) | 指示是否应应用字体格式。 |
| [SetIsFontApplied](./setisfontapplied/) | 指示是否应应用字体格式。 |
| [IsAlignmentApplied](./isalignmentapplied/) | 指示是否应应用对齐格式。 |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | 指示是否应应用对齐格式。 |
| [IsBorderApplied](./isborderapplied/) | 指示是否应应用边框格式。 |
| [SetIsBorderApplied](./setisborderapplied/) | 指示是否应应用边框格式。 |
| [IsFillApplied](./isfillapplied/) | 指示是否应应用填充格式。 |
| [SetIsFillApplied](./setisfillapplied/) | 指示是否应应用填充格式。 |
| [IsProtectionApplied](./isprotectionapplied/) | 指示是否应应用保护格式。 |
| [SetIsProtectionApplied](./setisprotectionapplied/) | 指示是否应应用保护格式。 |
| [IsModified](./ismodified/) | 检查样式的指定属性是否已被修改。用于 ConditionalFormattings 的样式，以检查在对单元格应用 ConditionalFormattings 时是否应使用该样式的指定属性。 |
| [Equals](./equals/) | 确定两个 Style 实例是否相等。 |
| [GetHashCode](./gethashcode/) | 作为 Style 对象的哈希函数。 |
| [GetIndentLevel](./getindentlevel/) | 表示单元格或范围的缩进级别。只能是 0 到 250 之间的整数。 |
| [SetIndentLevel](./setindentlevel/) | 表示单元格或范围的缩进级别。只能是 0 到 250 之间的整数。 |
| [GetFont](./getfont/) | 获取 Font 对象。 |
| [GetRotationAngle](./getrotationangle/) | 表示文本旋转角度。 |
| [SetRotationAngle](./setrotationangle/) | 表示文本旋转角度。 |
| [GetHorizontalAlignment](./gethorizontalalignment/) | 获取或设置单元格中文本的水平对齐类型。 |
| [SetHorizontalAlignment](./sethorizontalalignment/) | 获取或设置单元格中文本的水平对齐类型。 |
| [GetVerticalAlignment](./getverticalalignment/) | 获取或设置单元格中文本的垂直对齐类型。 |
| [SetVerticalAlignment](./setverticalalignment/) | 获取或设置单元格中文本的垂直对齐类型。 |
| [IsTextWrapped](./istextwrapped/) | 获取或设置一个值，指示单元格内的文本是否换行。 |
| [SetIsTextWrapped](./setistextwrapped/) | 获取或设置一个值，指示单元格内的文本是否换行。 |
| [GetNumber](./getnumber/) | 获取或设置数字和日期的显示格式。不同地区的格式模式不同。 |
| [SetNumber](./setnumber/) | 获取或设置数字和日期的显示格式。不同地区的格式模式不同。 |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | 设置样式的边框。 |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | 设置样式的边框。 |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | 设置外框边框 |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | 设置外框边框 |
| [IsLocked](./islocked/) | 获取或设置一个值，指示单元格是否可以被修改。 |
| [SetIsLocked](./setislocked/) | 获取或设置一个值，指示单元格是否可以被修改。 |
| [SetCustom_String_Bool](./setcustom_string_bool/) | 设置单元格的自定义数字格式字符串。 |
| [GetCustom](./getcustom/) | 表示此样式对象的自定义数字格式字符串。如果未设置自定义数字格式（例如，数字格式为内置），将返回空字符串 \"\"。 |
| [SetCustom_String](./setcustom_string/) | 表示此样式对象的自定义数字格式字符串。如果未设置自定义数字格式（例如，数字格式为内置），将返回空字符串 \"\"。 |
| [GetCultureCustom](./getculturecustom/) | 获取和设置与区域文化相关的数字格式模式字符串。如果此对象未设置数字格式，将返回 null。如果数字格式为内置，将返回对应于内置数字的模式字符串。 |
| [SetCultureCustom](./setculturecustom/) | 获取和设置与区域文化相关的数字格式模式字符串。如果此对象未设置数字格式，将返回 null。如果数字格式为内置，将返回对应于内置数字的模式字符串。 |
| [GetInvariantCustom](./getinvariantcustom/) | 获取与区域文化无关的数字格式模式字符串。如果此对象未设置数字格式，将返回 null。如果数字格式为内置，将返回对应于内置数字的模式字符串。 |
| [IsFormulaHidden](./isformulahidden/) | 表示在工作表受保护时公式是否会被隐藏。 |
| [SetIsFormulaHidden](./setisformulahidden/) | 表示在工作表受保护时公式是否会被隐藏。 |
| [GetShrinkToFit](./getshrinktofit/) | 表示文本是否会自动缩小以适应可用的列宽。 |
| [SetShrinkToFit](./setshrinktofit/) | 表示文本是否会自动缩小以适应可用的列宽。 |
| [GetTextDirection](./gettextdirection/) | 表示文本的阅读顺序。 |
| [SetTextDirection](./settextdirection/) | 表示文本的阅读顺序。 |
| [IsJustifyDistributed](./isjustifydistributed/) | 指示在文本的最后一行是否应使用两端对齐或分散对齐。 |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | 指示在文本的最后一行是否应使用两端对齐或分散对齐。 |
| [GetQuotePrefix](./getquoteprefix/) | 指示单元格的值是否以单引号开头。 |
| [SetQuotePrefix](./setquoteprefix/) | 指示单元格的值是否以单引号开头。 |
| [IsGradient](./isgradient/) | 指示单元格的填充是否为渐变图案。 |
| [SetIsGradient](./setisgradient/) | 指示单元格的填充是否为渐变图案。 |
| [SetTwoColorGradient](./settwocolorgradient/) | 将指定的填充设置为双颜色渐变。 |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | 获取双颜色渐变设置。 |
| [IsPercent](./ispercent/) | 指示数字格式是否为百分比格式。 |
| [IsDateTime](./isdatetime/) | 指示数字格式是否为日期格式。 |
| [IsCheckBox](./ischeckbox/) | 指示它是否为复选框样式 |
| [SetIsCheckBox](./setischeckbox/) | 指示它是否为复选框样式 |
| [ToJson](./tojson/) | 将样式转换为 JSON 结构数据。 |
| [GetLeftBorder](./getleftborder/) | 获取左边框。 |
| [GetRightBorder](./getrightborder/) | 获取右边框。 |
| [GetTopBorder](./gettopborder/) | 获取顶部边框。 |
| [GetBottomBorder](./getbottomborder/) | 获取底部边框。 |
