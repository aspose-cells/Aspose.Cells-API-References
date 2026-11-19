---
title: "Style"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 Excel 文档的显示样式，例如字体颜色、对齐、边框等。"
type: docs
url: /zh/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

表示 Excel 文档的显示样式，例如字体、颜色、对齐、边框等。Style 对象将所有样式属性（字体、数字格式、对齐等）作为属性。

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Style()](#Style--) | 初始化一个新的 [Style](../../com.aspose.cells/style) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | 从另一个样式对象复制数据 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定两个 Style 实例是否相等。 |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | 获取具有 32 位 ARGB 值的背景颜色。 |
| [getBackgroundColor()](#getBackgroundColor--) | 获取样式的背景颜色。 |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | 获取背景主题颜色。 |
| [getBorders()](#getBorders--) | 获取样式的 [BorderCollection](../../com.aspose.cells/bordercollection)。 |
| [getBottomBorder()](#getBottomBorder--) | 获取底部边框。 |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | 获取与区域设置相关的数字格式模式字符串。 |
| [getCustom()](#getCustom--) | 表示此样式对象的自定义数字格式字符串。 |
| [getFont()](#getFont--) | 获取一个 [getFont()](../../com.aspose.cells/style\#getFont--) 对象。 |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | 获取具有 32 位 ARGB 值的前景颜色。 |
| [getForegroundColor()](#getForegroundColor--) | 获取样式的前景颜色。 |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | 获取前景主题颜色。 |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | 获取单元格中文本的水平对齐类型。 |
| [getIndentLevel()](#getIndentLevel--) | 表示单元格或范围的缩进级别。 |
| [getInvariantCustom()](#getInvariantCustom--) | 获取与区域设置无关的数字格式模式字符串。 |
| [getLeftBorder()](#getLeftBorder--) | 获取左侧边框。 |
| [getName()](#getName--) | 获取样式的名称。 |
| [getNumber()](#getNumber--) | 获取数字和日期的显示格式。 |
| [getParentStyle()](#getParentStyle--) | 获取此样式的父样式。 |
| [getPattern()](#getPattern--) | 获取单元格背景图案类型。 |
| [getQuotePrefix()](#getQuotePrefix--) | 指示单元格的值是否以单引号开头。 |
| [getRightBorder()](#getRightBorder--) | 获取右侧边框。 |
| [getRotationAngle()](#getRotationAngle--) | 表示文本旋转角度。 |
| [getShrinkToFit()](#getShrinkToFit--) | 表示文本是否自动缩小以适应可用列宽。 |
| [getTextDirection()](#getTextDirection--) | 表示文本阅读顺序。 |
| [getTopBorder()](#getTopBorder--) | 获取上边框。 |
| [getTwoColorGradient()](#getTwoColorGradient--) | 获取双色渐变设置。 |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | 获取双色渐变设置。 |
| [getVerticalAlignment()](#getVerticalAlignment--) | 获取单元格中文本的垂直对齐类型。 |
| [hasBorders()](#hasBorders--) | 检查样式是否已设置边框。 |
| [hashCode()](#hashCode--) | 作为 Style 对象的哈希函数。 |
| [isAlignmentApplied()](#isAlignmentApplied--) | 指示是否应应用对齐格式。 |
| [isBorderApplied()](#isBorderApplied--) | 指示是否应应用边框格式。 |
| [isCheckBox()](#isCheckBox--) | 指示它是否为复选框样式 |
| [isDateTime()](#isDateTime--) | 指示数字格式是否为日期格式。 |
| [isFillApplied()](#isFillApplied--) | 指示是否应应用填充格式。 |
| [isFontApplied()](#isFontApplied--) | 指示是否应应用字体格式。 |
| [isFormulaHidden()](#isFormulaHidden--) | 表示在工作表受保护时公式是否会被隐藏。 |
| [isGradient()](#isGradient--) | 指示单元格着色是否为渐变图案。 |
| [isJustifyDistributed()](#isJustifyDistributed--) | 指示是否应在文本最后一行使用两端对齐或分散对齐。 |
| [isLocked()](#isLocked--) | 获取指示单元格是否可修改的值。 |
| [isModified(int modifyFlag)](#isModified-int-) | 检查样式的指定属性是否已被修改。 |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | 指示是否应应用数字格式。 |
| [isPercent()](#isPercent--) | 指示数字格式是否为百分比格式。 |
| [isProtectionApplied()](#isProtectionApplied--) | 指示是否应应用保护格式。 |
| [isTextWrapped()](#isTextWrapped--) | 获取指示单元格内文本是否换行的值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | 指示是否应应用对齐格式。 |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | 使用 32 位 ARGB 值设置背景颜色。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | 设置样式的背景颜色。 |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | 设置背景主题颜色。 |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | 设置样式的边框。 |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | 设置样式的边框。 |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | 指示是否应应用边框格式。 |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | 指示它是否为复选框样式 |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | 设置与区域相关的数字格式模式字符串。 |
| [setCustom(String value)](#setCustom-java.lang.String-) | 表示此样式对象的自定义数字格式字符串。 |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | 设置单元格的自定义数字格式字符串。 |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | 指示是否应应用填充格式。 |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | 指示是否应应用字体格式。 |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | 使用 32 位 ARGB 值设置前景色。 |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | 设置样式的前景色。 |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | 设置前景主题颜色。 |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | 表示在工作表受保护时公式是否会被隐藏。 |
| [setGradient(boolean value)](#setGradient-boolean-) | 指示单元格着色是否为渐变图案。 |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | 设置单元格中文本的水平对齐方式。 |
| [setIndentLevel(int value)](#setIndentLevel-int-) | 表示单元格或范围的缩进级别。 |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | 指示是否应在文本最后一行使用两端对齐或分散对齐。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 设置一个值，指示单元格是否可以被修改。 |
| [setName(String value)](#setName-java.lang.String-) | 设置样式的名称。 |
| [setNumber(int value)](#setNumber-int-) | 设置数字和日期的显示格式。 |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | 指示是否应应用数字格式。 |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | 设置轮廓边框 |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | 设置轮廓边框 |
| [setPattern(int value)](#setPattern-int-) | 设置单元格背景图案类型。 |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | 设置背景颜色。 |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | 指示是否应应用保护格式。 |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | 指示单元格的值是否以单引号开头。 |
| [setRotationAngle(int value)](#setRotationAngle-int-) | 表示文本旋转角度。 |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | 表示文本是否自动缩小以适应可用列宽。 |
| [setTextDirection(int value)](#setTextDirection-int-) | 表示文本阅读顺序。 |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | 设置一个值，指示单元格内的文本是否换行。 |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | 将指定填充设置为双色渐变。 |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | 设置单元格中文本的垂直对齐方式。 |
| [toJson()](#toJson--) | 将 [Style](../../com.aspose.cells/style) 转换为 JSON 结构数据。 |
| [toString()](#toString--) |  |
| [update()](#update--) | 将命名样式应用于使用该命名样式的单元格的样式。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


初始化一个新的 [Style](../../com.aspose.cells/style) 类实例。

**Remarks**

注意：此构造函数已过时。请改用 CellsFactory.CreateStyle() 方法。此属性将在 2016 年 10 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


从另一个样式对象复制数据

**Remarks**

此方法不会复制样式的名称。如果您想复制名称，请在复制样式后调用以下代码：destStyle.Name = style.Name。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 源 Style 对象 |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定两个 Style 实例是否相等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与当前 Style 对象比较的 Style 对象。 |

**Returns:**
boolean - 如果指定的对象等于当前对象则为 true；否则为 false。
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


获取具有 32 位 ARGB 值的背景颜色。

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


获取样式的背景颜色。

**Remarks**

如果您想设置单元格的颜色，请使用 Style.ForegroundColor 属性。仅当单元格样式图案不是 none 或 solid 时，此属性才会生效。

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


获取背景主题颜色。

**Remarks**

如果背景颜色不是主题颜色，将返回 NULL。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


获取样式的 [BorderCollection](../../com.aspose.cells/bordercollection)。

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


获取底部边框。

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


获取与区域相关的数字格式模式字符串。如果此对象未设置数字格式，则返回 null。如果数字格式是内置的，则返回对应内置数字的模式字符串。

**Remarks**

对于内置数字格式，模式内容（例如，某些地区的内置日期格式为 "m/d/y"，而其他地区则为 "d/m/y"）和格式说明符（例如，某些地区使用除 'y' 之外的字符来表示日期格式中的年份部分）均受文化差异影响；对于用户指定的自定义格式，仅会根据文化更改格式说明符，格式模式的其他部分不会被修改。

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


表示此样式对象的自定义数字格式字符串。如果未设置自定义数字格式（例如，数字格式为内置），将返回空字符串 ""。

**Remarks**

返回的自定义字符串与文化无关。

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


获取一个 [getFont()](../../com.aspose.cells/style\#getFont--) 对象。

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


获取具有 32 位 ARGB 值的前景颜色。

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


获取样式的前景颜色。

**Remarks**

如果返回 Color.Empty，则表示未设置颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


获取前景主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


获取单元格中文本的水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


表示单元格或范围的缩进级别。只能是 0 到 250 的整数。

**Remarks**

如果文本水平对齐类型设置为除左或右之外的值，缩进级别将重置为零。

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


获取与文化无关的数字格式模式字符串。如果此对象未设置数字格式，将返回 null。如果数字格式为内置，则返回对应于内置数字的模式字符串。

**Remarks**

对于内置数字格式，返回的模式内容仍然受文化差异影响，例如，对于某些地区返回 "m/d/y"，而对其他地区返回 "d/m/y"。与 [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) 的区别在于（这也是文化无关的含义）：格式说明符和分隔符保持为标准形式，例如 '/' 始终用作日期时间分隔符，且 "y" 始终用作 "年份" 部分，无论特定地区使用何种其他特殊字符。

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


获取左侧边框。

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


获取样式的名称。

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


获取数字和日期的显示格式。不同地区的格式模式各不相同。

**Remarks**

例如，针对 en\_US 区域的数字所表示的格式模式如下：

| 值 | 类型 | 格式字符串 |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


获取此样式的父样式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


获取单元格背景图案类型。

请参阅 [BackgroundType](../../com.aspose.cells/backgroundtype)。

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


指示单元格的值是否以单引号开头。

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


获取右侧边框。

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


表示文本旋转角度。

**Remarks**

0：未旋转。

255：从上到下。

\-90：向下。

90：向上。

您可以设置 255 或范围在 -90 到 90 之间的值。

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


表示文本是否自动缩小以适应可用列宽。

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


获取上边框。

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


获取双色渐变设置。

**Remarks**

注意：此方法现已过时。请改用 Style.GetTwoColorGradientSetting() 方法。此属性将在自 2022 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.Object[] - 返回关于双色渐变的所有设置 [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


获取双色渐变设置。

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


获取单元格中文本的垂直对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


检查样式是否已设置边框。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为 Style 对象的哈希函数。

**Remarks**

此方法仅供内部使用。

**Returns:**
int - 当前对象的哈希码。
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


指示是否应应用对齐格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


指示是否应应用边框格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


指示它是否为复选框样式

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


指示数字格式是否为日期格式。

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


指示是否应应用填充格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


指示是否应应用字体格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


表示在工作表受保护时公式是否会被隐藏。

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


指示单元格着色是否为渐变图案。

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


指示是否应在文本最后一行使用两端对齐或分散对齐。

**Remarks**

这在东亚对齐中很常见，但在其他情况下并不常见。仅在分布式 dorizontal 对齐时有效。

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


获取指示单元格是否可修改的值。

**Remarks**

锁定单元格在工作表未受保护时无效。

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


检查样式的指定属性是否已被修改。用于 ConditionalFormattings 的样式，以检查在对单元格应用 ConditionalFormattings 时是否应使用此样式的指定属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). 样式修改标志 |

**Returns:**
boolean - 如果指定属性已被修改则为 true
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


指示是否应应用数字格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


指示数字格式是否为百分比格式。

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


指示是否应应用保护格式。

**Remarks**

仅用于命名样式。

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


获取指示单元格内文本是否换行的值。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


指示是否应应用对齐格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


使用 32 位 ARGB 值设置背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


设置样式的背景颜色。

**Remarks**

如果您想设置单元格的颜色，请使用 Style.ForegroundColor 属性。仅当单元格样式图案不是 none 或 solid 时，此属性才会生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


设置背景主题颜色。

**Remarks**

如果背景颜色不是主题颜色，将返回 NULL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


设置样式的边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). 要设置的边框，可为 [BorderType](../../com.aspose.cells/bordertype) 的组合。 |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). 边框的样式。 |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | 边框的颜色。 |

**Returns:**
boolean - 当前边框设置是否已更改。
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


设置样式的边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). 要设置的边框，可为 [BorderType](../../com.aspose.cells/bordertype) 的组合。 |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). 边框的样式。 |
| borderColor | [Color](../../com.aspose.cells/color) | 边框的颜色。 |

**Returns:**
boolean - 当前边框设置是否已更改。
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


指示是否应应用边框格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


指示它是否为复选框样式

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


设置与区域文化相关的数字格式模式字符串。如果此对象未设置数字格式，则返回 null。如果数字格式是内置的，则返回对应内置数字的模式字符串。

**Remarks**

对于内置数字格式，模式内容（例如，某些地区的内置日期格式为 "m/d/y"，而其他地区则为 "d/m/y"）和格式说明符（例如，某些地区使用除 'y' 之外的字符来表示日期格式中的年份部分）均受文化差异影响；对于用户指定的自定义格式，仅会根据文化更改格式说明符，格式模式的其他部分不会被修改。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


表示此样式对象的自定义数字格式字符串。如果未设置自定义数字格式（例如，数字格式为内置），将返回空字符串 ""。

**Remarks**

返回的自定义字符串与文化无关。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


设置单元格的自定义数字格式字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 自定义 | java.lang.String | 自定义数字格式字符串，应为 InvariantCulture 模式。 |
| 内置首选项 | boolean | 如果给定的自定义数字格式字符串匹配当前区域设置对应的内置数字格式之一，则是否将数字格式设置为内置而非自定义。 |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


指示是否应应用填充格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


指示是否应应用字体格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


使用 32 位 ARGB 值设置前景色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


设置样式的前景色。

**Remarks**

如果返回 Color.Empty，则表示未设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


设置前景主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


表示在工作表受保护时公式是否会被隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


指示单元格着色是否为渐变图案。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


设置单元格中文本的水平对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


表示单元格或范围的缩进级别。只能是 0 到 250 的整数。

**Remarks**

如果文本水平对齐类型设置为除左或右之外的值，缩进级别将重置为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


指示是否应在文本最后一行使用两端对齐或分散对齐。

**Remarks**

这在东亚对齐中很常见，但在其他情况下并不常见。仅在分布式 dorizontal 对齐时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


设置一个值，指示单元格是否可以被修改。

**Remarks**

锁定单元格在工作表未受保护时无效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置样式的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


设置数字和日期的显示格式。不同地区的格式模式不同。

**Remarks**

例如，针对 en\_US 区域的数字所表示的格式模式如下：

| 值 | 类型 | 格式字符串 |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


指示是否应应用数字格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


设置轮廓边框

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). 边框的类型。 |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | 边框的颜色 |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


设置轮廓边框

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). 边框的类型。 |
| borderColor | [Color](../../com.aspose.cells/color) | 边框的颜色 |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


设置单元格背景图案类型。

请参阅 [BackgroundType](../../com.aspose.cells/backgroundtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


设置背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). 图案。 |
| color1 | [Color](../../com.aspose.cells/color) | 前景色。 |
| color2 | [Color](../../com.aspose.cells/color) | 背景颜色。仅在图案不是 BackgroundType.None 且为 BackgroundType.Solid 时有效。 |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


指示是否应应用保护格式。

**Remarks**

仅用于命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


指示单元格的值是否以单引号开头。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


表示文本旋转角度。

**Remarks**

0：未旋转。

255：从上到下。

\-90：向下。

90：向上。

您可以设置 255 或范围在 -90 到 90 之间的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


表示文本是否自动缩小以适应可用列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


设置一个值，指示单元格内的文本是否换行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


将指定填充设置为双色渐变。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| color2 | [Color](../../com.aspose.cells/color) | 双色渐变。 |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


设置单元格中文本的垂直对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


将 [Style](../../com.aspose.cells/style) 转换为 JSON 结构数据。

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


将命名样式应用于使用该命名样式的单元格的样式。它的作用类似于在完成样式修改后点击 "ok" 按钮。仅适用于命名样式。

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

