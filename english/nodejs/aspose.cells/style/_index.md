---
title: "Style"
linktitle: "Style"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents display style of excel document,such as font,color,alignment,border,etc."
type: docs
weight: 3940
url: /nodejs/aspose.cells/style/
---

## Style class

Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties.

```js
new Style()
```

Initializes a new instance of the Style class. NOTE: This constructor is now obsolete. Instead, please use CellsFactory.CreateStyle() method. This property will be removed 6 months later since October 2016. Aspose apologizes for any inconvenience you may have experienced.

## Methods

| Name | Description |
| --- | --- |
| [copy(style)](#copy) | Copies data from another style object This method does not copy the name of the style. If you want to copy the name, ple |
| [equals(obj)](#equals) | Determines whether two Style instances are equal. |
| [getBackgroundArgbColor()](#getbackgroundargbcolor) | Gets and sets the background color with a 32-bit ARGB value. |
| [getBackgroundColor()](#getbackgroundcolor) | Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. O |
| [getBackgroundThemeColor()](#getbackgroundthemecolor) | Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned. |
| [getBorders()](#getborders) | Gets the BorderCollection of the style. |
| [getBottomBorder()](#getbottomborder) |  |
| [getCultureCustom()](#getculturecustom) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object,  |
| [getCustom()](#getcustom) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the |
| [getFont()](#getfont) | Gets a Font object. |
| [getForegroundArgbColor()](#getforegroundargbcolor) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [getForegroundColor()](#getforegroundcolor) | Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned. |
| [getForegroundThemeColor()](#getforegroundthemecolor) | Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned. |
| [getHorizontalAlignment()](#gethorizontalalignment) | Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer |
| [getIndentLevel()](#getindentlevel) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment ty |
| [getInvariantCustom()](#getinvariantcustom) | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null wi |
| [getLeftBorder()](#getleftborder) |  |
| [getName()](#getname) | Gets or sets the name of the style. |
| [getNumber()](#getnumber) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For e |
| [getParentStyle()](#getparentstyle) | Gets the parent style of this style. |
| [getPattern()](#getpattern) | Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant. |
| [getQuotePrefix()](#getquoteprefix) | Indicates whether the cell's value starts with single quote mark. |
| [getRightBorder()](#getrightborder) |  |
| [getRotationAngle()](#getrotationangle) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ran |
| [getShrinkToFit()](#getshrinktofit) | Represents if text automatically shrinks to fit in the available column width. |
| [getTextDirection()](#gettextdirection) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [getTopBorder()](#gettopborder) |  |
| [getTwoColorGradient()](#gettwocolorgradient) | Get the two-color gradient setting. If this is not gradient fill,return null; NOTE: This method is now obsolete. Instead |
| [getTwoColorGradientSetting()](#gettwocolorgradientsetting) | Get the two-color gradient setting. |
| [getVerticalAlignment()](#getverticalalignment) | Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer c |
| [hasBorders()](#hasborders) | Checks whether there are borders have been set for the style. |
| [hashCode()](#hashcode) | Serves as a hash function for a Style object. This method is only for internal use.@return {Number} A hash code for the  |
| [isAlignmentApplied()](#isalignmentapplied) | Indicate whether the alignment formatting should be applied. Only for named style. |
| [isBorderApplied()](#isborderapplied) | Indicate whether the border formatting should be applied. Only for named style. |
| [isCheckBox()](#ischeckbox) |  |
| [isDateTime()](#isdatetime) | Indicates whether the number format is a date format. |
| [isFillApplied()](#isfillapplied) | Indicate whether the fill formatting should be applied. Only for named style. |
| [isFontApplied()](#isfontapplied) | Indicate whether the font formatting should be applied. Only for named style. |
| [isFormulaHidden()](#isformulahidden) | Represents if the formula will be hidden when the worksheet is protected. |
| [isGradient()](#isgradient) | Indicates whether the cell shading is a gradient pattern. |
| [isJustifyDistributed()](#isjustifydistributed) | Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for E |
| [isLocked()](#islocked) | Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet  |
| [isModified(modifyFlag)](#ismodified) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to che |
| [isNumberFormatApplied()](#isnumberformatapplied) | Indicate whether the number formatting should be applied. Only for named style. |
| [isPercent()](#ispercent) | Indicates whether the number format is a percent format. |
| [isProtectionApplied()](#isprotectionapplied) | Indicate whether the protection formatting should be applied. Only for named style. |
| [isTextWrapped()](#istextwrapped) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [setAlignmentApplied()](#setalignmentapplied) | Indicate whether the alignment formatting should be applied. Only for named style. |
| [setBackgroundArgbColor()](#setbackgroundargbcolor) | Gets and sets the background color with a 32-bit ARGB value. |
| [setBackgroundColor()](#setbackgroundcolor) | Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. O |
| [setBackgroundThemeColor()](#setbackgroundthemecolor) | Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned. |
| [setBorder(borderType, borderStyle, borderColor)](#setborder) | Sets the borders of the style. |
| [setBorder(borderType, borderStyle, borderColor)](#setborder-1) | Sets the borders of the style. |
| [setBorderApplied()](#setborderapplied) | Indicate whether the border formatting should be applied. Only for named style. |
| [setCheckBox()](#setcheckbox) |  |
| [setCultureCustom()](#setculturecustom) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object,  |
| [setCustom()](#setcustom) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the |
| [setCustom(custom, builtinPreference)](#setcustom-1) | Sets the Custom number format string of a cell. |
| [setFillApplied()](#setfillapplied) | Indicate whether the fill formatting should be applied. Only for named style. |
| [setFontApplied()](#setfontapplied) | Indicate whether the font formatting should be applied. Only for named style. |
| [setForegroundArgbColor()](#setforegroundargbcolor) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [setForegroundColor()](#setforegroundcolor) | Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned. |
| [setForegroundThemeColor()](#setforegroundthemecolor) | Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned. |
| [setFormulaHidden()](#setformulahidden) | Represents if the formula will be hidden when the worksheet is protected. |
| [setGradient()](#setgradient) | Indicates whether the cell shading is a gradient pattern. |
| [setHorizontalAlignment()](#sethorizontalalignment) | Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer |
| [setIndentLevel()](#setindentlevel) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment ty |
| [setJustifyDistributed()](#setjustifydistributed) | Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for E |
| [setLocked()](#setlocked) | Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet  |
| [setName()](#setname) | Gets or sets the name of the style. |
| [setNumber()](#setnumber) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For e |
| [setNumberFormatApplied()](#setnumberformatapplied) | Indicate whether the number formatting should be applied. Only for named style. |
| [setPattern()](#setpattern) | Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant. |
| [setPatternColor(pattern, color1, color2)](#setpatterncolor) | Sets the background color. |
| [setProtectionApplied()](#setprotectionapplied) | Indicate whether the protection formatting should be applied. Only for named style. |
| [setQuotePrefix()](#setquoteprefix) | Indicates whether the cell's value starts with single quote mark. |
| [setRotationAngle()](#setrotationangle) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ran |
| [setShrinkToFit()](#setshrinktofit) | Represents if text automatically shrinks to fit in the available column width. |
| [setTextDirection()](#settextdirection) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [setTextWrapped()](#settextwrapped) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [setTwoColorGradient(color1, color2, gradientStyleType, variant)](#settwocolorgradient) | Sets the specified fill to a two-color gradient. |
| [setVerticalAlignment()](#setverticalalignment) | Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer c |
| [toJson()](#tojson) | Convert Style to JSON struct data. |
| [update()](#update) | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button afte |

### copy(style) {#copy}

Copies data from another style object This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |

### equals(obj) {#equals}

Determines whether two Style instances are equal.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The Style object to compare with the current Style object. |

**Returns:** boolean — `boolean` true if the specified Object is equal to the current Object; otherwise, false.

### getBackgroundArgbColor() {#getbackgroundargbcolor}

Gets and sets the background color with a 32-bit ARGB value.

### getBackgroundColor() {#getbackgroundcolor}

Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### getBackgroundThemeColor() {#getbackgroundthemecolor}

Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned.

### getBorders() {#getborders}

Gets the BorderCollection of the style.

### getBottomBorder() {#getbottomborder}

### getCultureCustom() {#getculturecustom}

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### getCustom() {#getcustom}

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. The returned custom string is culture-independent.

### getFont() {#getfont}

Gets a Font object.

### getForegroundArgbColor() {#getforegroundargbcolor}

Gets and sets the foreground color with a 32-bit ARGB value.

### getForegroundColor() {#getforegroundcolor}

Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned.

### getForegroundThemeColor() {#getforegroundthemecolor}

Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned.

### getHorizontalAlignment() {#gethorizontalalignment}

Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

### getIndentLevel() {#getindentlevel}

Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### getInvariantCustom() {#getinvariantcustom}

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from CultureCustom is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.

### getLeftBorder() {#getleftborder}

### getName() {#getname}

Gets or sets the name of the style.

### getNumber() {#getnumber}

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For example, the formatting patterns represented by numbers for en_US region: ValueTypeFormat String0GeneralGeneral1Decimal02Decimal0.003Decimal#,##04Decimal#,##0.005Currency$#,##0_);($#,##0)6Currency$#,##0_); Red 7Currency$#,##0.00_);($#,##0.00)8Currency$#,##0.00_); Red 9Percentage0%10Percentage0.00%11Scientific0.00E+0012Fraction# ?/?13Fraction# ??/??14Datem/d/yyyy15Dated-mmm-yy16Dated-mmm17Datemmm-yy18Timeh:mm AM/PM19Timeh:mm:ss AM/PM20Timeh:mm21Timeh:mm:ss22Timem/d/yyyy h:mm37Accounting#,##0_);(#,##0)38Accounting#,##0_); Red 39Accounting#,##0.00_);(#,##0.00)40Accounting#,##0.00_); Red 41Accounting_(* #,##0_); (* (#,##0); (* "-" ); (@ )42Currency ($* #,##0_); ($* (#,##0); ($* "-" ); (@ )43Accounting (* #,##0.00_); (* (#,##0.00); (* "-"?? ); (@ )44Currency ($* #,##0.00_); ($* (#,##0.00); ($* "-"?? ); (@_)45Timemm:ss46Time[h]:mm:ss47Timemm:ss.048Scientific##0.0E+049Text@

### getParentStyle() {#getparentstyle}

Gets the parent style of this style.

### getPattern() {#getpattern}

Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant.

### getQuotePrefix() {#getquoteprefix}

Indicates whether the cell's value starts with single quote mark.

### getRightBorder() {#getrightborder}

### getRotationAngle() {#getrotationangle}

Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ranged from -90 to 90.

### getShrinkToFit() {#getshrinktofit}

Represents if text automatically shrinks to fit in the available column width.

### getTextDirection() {#gettextdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant.

### getTopBorder() {#gettopborder}

### getTwoColorGradient() {#gettwocolorgradient}

Get the two-color gradient setting. If this is not gradient fill,return null; NOTE: This method is now obsolete. Instead, please use Style.GetTwoColorGradientSetting() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {Object[]} Returns all setting about two-color gradient [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant

### getTwoColorGradientSetting() {#gettwocolorgradientsetting}

Get the two-color gradient setting.

### getVerticalAlignment() {#getverticalalignment}

Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

### hasBorders() {#hasborders}

Checks whether there are borders have been set for the style.

### hashCode() {#hashcode}

Serves as a hash function for a Style object. This method is only for internal use.@return {Number} A hash code for the current Object.

### isAlignmentApplied() {#isalignmentapplied}

Indicate whether the alignment formatting should be applied. Only for named style.

### isBorderApplied() {#isborderapplied}

Indicate whether the border formatting should be applied. Only for named style.

### isCheckBox() {#ischeckbox}

### isDateTime() {#isdatetime}

Indicates whether the number format is a date format.

### isFillApplied() {#isfillapplied}

Indicate whether the fill formatting should be applied. Only for named style.

### isFontApplied() {#isfontapplied}

Indicate whether the font formatting should be applied. Only for named style.

### isFormulaHidden() {#isformulahidden}

Represents if the formula will be hidden when the worksheet is protected.

### isGradient() {#isgradient}

Indicates whether the cell shading is a gradient pattern.

### isJustifyDistributed() {#isjustifydistributed}

Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for East Asian alignments but not typical in other contexts.

### isLocked() {#islocked}

Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet is protected.

### isModified(modifyFlag) {#ismodified}

Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | Number | StyleModifyFlag |

**Returns:** boolean — `boolean` true if the specified properties have been modified

### isNumberFormatApplied() {#isnumberformatapplied}

Indicate whether the number formatting should be applied. Only for named style.

### isPercent() {#ispercent}

Indicates whether the number format is a percent format.

### isProtectionApplied() {#isprotectionapplied}

Indicate whether the protection formatting should be applied. Only for named style.

### isTextWrapped() {#istextwrapped}

Gets or sets a value indicating whether the text within a cell is wrapped.

### setAlignmentApplied() {#setalignmentapplied}

Indicate whether the alignment formatting should be applied. Only for named style.

### setBackgroundArgbColor() {#setbackgroundargbcolor}

Gets and sets the background color with a 32-bit ARGB value.

### setBackgroundColor() {#setbackgroundcolor}

Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### setBackgroundThemeColor() {#setbackgroundthemecolor}

Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned.

### setBorder(borderType, borderStyle, borderColor) {#setborder}

Sets the borders of the style.

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | Number | BorderType |
| borderStyle | Number | CellBorderType |
| borderColor | Color | The color of the border. |

**Returns:** boolean — `boolean` Whether current border settings have been changed.

### setBorder(borderType, borderStyle, borderColor) {#setborder-1}

Sets the borders of the style.

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | Number | BorderType |
| borderStyle | Number | CellBorderType |
| borderColor | CellsColor | The color of the border. |

**Returns:** boolean — `boolean` Whether current border settings have been changed.

### setBorderApplied() {#setborderapplied}

Indicate whether the border formatting should be applied. Only for named style.

### setCheckBox() {#setcheckbox}

### setCultureCustom() {#setculturecustom}

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### setCustom() {#setcustom}

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. The returned custom string is culture-independent.

### setCustom(custom, builtinPreference) {#setcustom-1}

Sets the Custom number format string of a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| custom | String | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | boolean | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |

### setFillApplied() {#setfillapplied}

Indicate whether the fill formatting should be applied. Only for named style.

### setFontApplied() {#setfontapplied}

Indicate whether the font formatting should be applied. Only for named style.

### setForegroundArgbColor() {#setforegroundargbcolor}

Gets and sets the foreground color with a 32-bit ARGB value.

### setForegroundColor() {#setforegroundcolor}

Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned.

### setForegroundThemeColor() {#setforegroundthemecolor}

Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned.

### setFormulaHidden() {#setformulahidden}

Represents if the formula will be hidden when the worksheet is protected.

### setGradient() {#setgradient}

Indicates whether the cell shading is a gradient pattern.

### setHorizontalAlignment() {#sethorizontalalignment}

Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

### setIndentLevel() {#setindentlevel}

Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### setJustifyDistributed() {#setjustifydistributed}

Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for East Asian alignments but not typical in other contexts.

### setLocked() {#setlocked}

Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet is protected.

### setName() {#setname}

Gets or sets the name of the style.

### setNumber() {#setnumber}

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For example, the formatting patterns represented by numbers for en_US region: ValueTypeFormat String0GeneralGeneral1Decimal02Decimal0.003Decimal#,##04Decimal#,##0.005Currency$#,##0_);($#,##0)6Currency$#,##0_); Red 7Currency$#,##0.00_);($#,##0.00)8Currency$#,##0.00_); Red 9Percentage0%10Percentage0.00%11Scientific0.00E+0012Fraction# ?/?13Fraction# ??/??14Datem/d/yyyy15Dated-mmm-yy16Dated-mmm17Datemmm-yy18Timeh:mm AM/PM19Timeh:mm:ss AM/PM20Timeh:mm21Timeh:mm:ss22Timem/d/yyyy h:mm37Accounting#,##0_);(#,##0)38Accounting#,##0_); Red 39Accounting#,##0.00_);(#,##0.00)40Accounting#,##0.00_); Red 41Accounting_(* #,##0_); (* (#,##0); (* "-" ); (@ )42Currency ($* #,##0_); ($* (#,##0); ($* "-" ); (@ )43Accounting (* #,##0.00_); (* (#,##0.00); (* "-"?? ); (@ )44Currency ($* #,##0.00_); ($* (#,##0.00); ($* "-"?? ); (@_)45Timemm:ss46Time[h]:mm:ss47Timemm:ss.048Scientific##0.0E+049Text@

### setNumberFormatApplied() {#setnumberformatapplied}

Indicate whether the number formatting should be applied. Only for named style.

### setPattern() {#setpattern}

Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant.

### setPatternColor(pattern, color1, color2) {#setpatterncolor}

Sets the background color.

| Parameter | Type | Description |
| --- | --- | --- |
| pattern | Number | BackgroundType |
| color1 | Color | The foreground color. |
| color2 | Color | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |

### setProtectionApplied() {#setprotectionapplied}

Indicate whether the protection formatting should be applied. Only for named style.

### setQuotePrefix() {#setquoteprefix}

Indicates whether the cell's value starts with single quote mark.

### setRotationAngle() {#setrotationangle}

Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ranged from -90 to 90.

### setShrinkToFit() {#setshrinktofit}

Represents if text automatically shrinks to fit in the available column width.

### setTextDirection() {#settextdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant.

### setTextWrapped() {#settextwrapped}

Gets or sets a value indicating whether the text within a cell is wrapped.

### setTwoColorGradient(color1, color2, gradientStyleType, variant) {#settwocolorgradient}

Sets the specified fill to a two-color gradient.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| gradientStyleType | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setVerticalAlignment() {#setverticalalignment}

Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

### toJson() {#tojson}

Convert Style to JSON struct data.

**Returns:** String — `String`

### update() {#update}

Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.
