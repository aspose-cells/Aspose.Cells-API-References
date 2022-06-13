---
title: Style
second_title: Aspose.Cells for .NET API 参考
description: 表示excel文档的显示风格如字体颜色对齐方式边框等
type: docs
weight: 5750
url: /zh/net/aspose.cells/style/
---
## Style class

表示excel文档的显示风格，如字体、颜色、对齐方式、边框等。

```csharp
public class Style
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | 使用 32 位 ARGB 值获取和设置背景颜色。 |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | 获取或设置样式的背景颜色。 |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | 获取和设置背景主题颜色。 |
| [Borders](../../aspose.cells/style/borders) { get; } | 获取样式的[`BorderCollection`](../bordercollection)。 |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | 获取和设置数字格式的文化相关模式字符串。 如果没有为此对象设置数字格式，则返回 null。 如果内置数字格式，则返回内置数字对应的模式字符串。 |
| [Custom](../../aspose.cells/style/custom) { get; set; } | 表示该样式对象的自定义数字格式字符串。 如果未设置自定义数字格式（例如内置数字格式），将返回“”。 |
| [Font](../../aspose.cells/style/font) { get; } | 获取[`Font`](./font)对象。 |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | 使用 32 位 ARGB 值获取和设置前景色。 |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | 获取或设置样式的前景色。 |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | 获取和设置前景主题颜色。 |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | 检查样式是否设置了边框。 |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | 获取或设置单元格中文本的水平对齐方式。 |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | 表示单元格或范围的缩进级别。只能是 0 到 250 之间的整数。 |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | 获取数字格式的与区域性无关的模式字符串。 如果没有为此对象设置数字格式，则返回 null。 如果内置数字格式，则返回内置数字对应的模式字符串。 |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | 表示数字格式是否为日期格式。 |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | 表示当工作表受到保护时公式是否隐藏。 |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | 指示单元格阴影是否为渐变图案。 |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | 指示单元格对齐或分布对齐是否应在文本的最后一行使用。 |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | 获取或设置一个值，指示是否可以修改单元格。 |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | 表示数字格式是否为百分比格式。 |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | 获取或设置一个值，该值指示单元格内的文本是否被换行。 |
| [Name](../../aspose.cells/style/name) { get; set; } | 获取或设置样式名称。 |
| [Number](../../aspose.cells/style/number) { get; set; } | 获取或设置数字和日期的显示格式。不同地区的格式模式不同。 |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | 获取该样式的父样式。 |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | 获取或设置单元格背景图案类型。 |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | 指示单元格的值是否以单引号开头。 |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | 代表文字旋转角度。 |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | 表示文本是否自动缩小以适应可用的列宽。 |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | 表示文本阅读顺序。 |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | 获取或设置单元格中文本的垂直对齐方式。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | 从另一个样式对象复制数据 |
| override [Equals](../../aspose.cells/style/equals)(object) | 确定两个 Style 实例是否相等。 |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | 用作 Style 对象的哈希函数。 |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | 获取双色渐变设置。 |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | 检查样式的指定属性是否已被修改。 用于 ConditionalFormattings 的样式，以检查在单元格上应用 ConditionalFormattings 时是否应使用此样式的指定属性。 |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | 设置样式的边框。 |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | 设置单元格的自定义数字格式字符串。 |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | 设置背景颜色。 |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | 将指定的填充设置为双色渐变。 |
| [Update](../../aspose.cells/style/update)() | 将命名样式应用于使用此命名样式的单元格的样式。 就像在完成样式修改后单击“确定”按钮一样。 仅适用于命名样式。 |

### 例子

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->