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
| [copy(style)](./copy/) | Copies data from another style object This method does not copy the name of the style. If you want to copy the name, ple |
| [equals(obj)](./equals/) | Determines whether two Style instances are equal. |
| [getBackgroundArgbColor()](./getbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
| [getBackgroundColor()](./getbackgroundcolor/) | Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. O |
| [getBackgroundThemeColor()](./getbackgroundthemecolor/) | Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned. |
| [getBorders()](./getborders/) | Gets the BorderCollection of the style. |
| [getBottomBorder()](./getbottomborder/) |  |
| [getCultureCustom()](./getculturecustom/) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object,  |
| [getCustom()](./getcustom/) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the |
| [getFont()](./getfont/) | Gets a Font object. |
| [getForegroundArgbColor()](./getforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [getForegroundColor()](./getforegroundcolor/) | Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned. |
| [getForegroundThemeColor()](./getforegroundthemecolor/) | Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned. |
| [getHorizontalAlignment()](./gethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer |
| [getIndentLevel()](./getindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment ty |
| [getInvariantCustom()](./getinvariantcustom/) | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null wi |
| [getLeftBorder()](./getleftborder/) |  |
| [getName()](./getname/) | Gets or sets the name of the style. |
| [getNumber()](./getnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For e |
| [getParentStyle()](./getparentstyle/) | Gets the parent style of this style. |
| [getPattern()](./getpattern/) | Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant. |
| [getQuotePrefix()](./getquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
| [getRightBorder()](./getrightborder/) |  |
| [getRotationAngle()](./getrotationangle/) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ran |
| [getShrinkToFit()](./getshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
| [getTextDirection()](./gettextdirection/) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [getTopBorder()](./gettopborder/) |  |
| [getTwoColorGradient()](./gettwocolorgradient/) | Get the two-color gradient setting. If this is not gradient fill,return null; NOTE: This method is now obsolete. Instead |
| [getTwoColorGradientSetting()](./gettwocolorgradientsetting/) | Get the two-color gradient setting. |
| [getVerticalAlignment()](./getverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer c |
| [hasBorders()](./hasborders/) | Checks whether there are borders have been set for the style. |
| [hashCode()](./hashcode/) | Serves as a hash function for a Style object. This method is only for internal use.@return {Number} A hash code for the  |
| [isAlignmentApplied()](./isalignmentapplied/) | Indicate whether the alignment formatting should be applied. Only for named style. |
| [isBorderApplied()](./isborderapplied/) | Indicate whether the border formatting should be applied. Only for named style. |
| [isCheckBox()](./ischeckbox/) |  |
| [isDateTime()](./isdatetime/) | Indicates whether the number format is a date format. |
| [isFillApplied()](./isfillapplied/) | Indicate whether the fill formatting should be applied. Only for named style. |
| [isFontApplied()](./isfontapplied/) | Indicate whether the font formatting should be applied. Only for named style. |
| [isFormulaHidden()](./isformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
| [isGradient()](./isgradient/) | Indicates whether the cell shading is a gradient pattern. |
| [isJustifyDistributed()](./isjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for E |
| [isLocked()](./islocked/) | Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet  |
| [isModified(modifyFlag)](./ismodified/) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to che |
| [isNumberFormatApplied()](./isnumberformatapplied/) | Indicate whether the number formatting should be applied. Only for named style. |
| [isPercent()](./ispercent/) | Indicates whether the number format is a percent format. |
| [isProtectionApplied()](./isprotectionapplied/) | Indicate whether the protection formatting should be applied. Only for named style. |
| [isTextWrapped()](./istextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [setAlignmentApplied()](./setalignmentapplied/) | Indicate whether the alignment formatting should be applied. Only for named style. |
| [setBackgroundArgbColor()](./setbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
| [setBackgroundColor()](./setbackgroundcolor/) | Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. O |
| [setBackgroundThemeColor()](./setbackgroundthemecolor/) | Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned. |
| [setBorder(borderType, borderStyle, borderColor)](./setborder/) | Sets the borders of the style. |
| [setBorder(borderType, borderStyle, borderColor)](./setborder-1/) | Sets the borders of the style. |
| [setBorderApplied()](./setborderapplied/) | Indicate whether the border formatting should be applied. Only for named style. |
| [setCheckBox()](./setcheckbox/) |  |
| [setCultureCustom()](./setculturecustom/) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object,  |
| [setCustom()](./setcustom/) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the |
| [setCustom(custom, builtinPreference)](./setcustom-1/) | Sets the Custom number format string of a cell. |
| [setFillApplied()](./setfillapplied/) | Indicate whether the fill formatting should be applied. Only for named style. |
| [setFontApplied()](./setfontapplied/) | Indicate whether the font formatting should be applied. Only for named style. |
| [setForegroundArgbColor()](./setforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [setForegroundColor()](./setforegroundcolor/) | Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned. |
| [setForegroundThemeColor()](./setforegroundthemecolor/) | Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned. |
| [setFormulaHidden()](./setformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
| [setGradient()](./setgradient/) | Indicates whether the cell shading is a gradient pattern. |
| [setHorizontalAlignment()](./sethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer |
| [setIndentLevel()](./setindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment ty |
| [setJustifyDistributed()](./setjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for E |
| [setLocked()](./setlocked/) | Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet  |
| [setName()](./setname/) | Gets or sets the name of the style. |
| [setNumber()](./setnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For e |
| [setNumberFormatApplied()](./setnumberformatapplied/) | Indicate whether the number formatting should be applied. Only for named style. |
| [setPattern()](./setpattern/) | Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant. |
| [setPatternColor(pattern, color1, color2)](./setpatterncolor/) | Sets the background color. |
| [setProtectionApplied()](./setprotectionapplied/) | Indicate whether the protection formatting should be applied. Only for named style. |
| [setQuotePrefix()](./setquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
| [setRotationAngle()](./setrotationangle/) | Represents text rotation angle. 0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward. You can set 255 or value ran |
| [setShrinkToFit()](./setshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
| [setTextDirection()](./settextdirection/) | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [setTextWrapped()](./settextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [setTwoColorGradient(color1, color2, gradientStyleType, variant)](./settwocolorgradient/) | Sets the specified fill to a two-color gradient. |
| [setVerticalAlignment()](./setverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer c |
| [toJson()](./tojson/) | Convert Style to JSON struct data. |
| [update()](./update/) | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button afte |
