---
title: "Style Class"
linktitle: "Style"
articleTitle: "Style"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents display style of excel document,such as font,color,alignment,border,etc."
type: docs
weight: 6410
url: /php/aspose.cells/style/
---

## Style class

Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties.

## Constructors

| Name | Description |
| --- | --- |
| [Style](#constructor) | Initializes a new instance of the Style class. NOTE: This constructor is now obsolete. Instead, please use CellsFactory. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [BackgroundThemeColor](#backgroundthemecolor) | ThemeColor | Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned. |
| [ForegroundThemeColor](#foregroundthemecolor) | ThemeColor | Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned. |
| [Name](#name) | String | Gets or sets the name of the style. |
| [Pattern](#pattern) | Number | Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant. |
| [Borders](#borders) | BorderCollection | Gets the BorderCollection of the style. |
| [BackgroundColor](#backgroundcolor) | Color | Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. O |
| [BackgroundArgbColor](#backgroundargbcolor) | Number | Gets and sets the background color with a 32-bit ARGB value. |
| [ForegroundColor](#foregroundcolor) | Color | Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned. |
| [ForegroundArgbColor](#foregroundargbcolor) | Number | Gets and sets the foreground color with a 32-bit ARGB value. |
| [HasBorders](#hasborders) | boolean | Checks whether there are borders have been set for the style. |
| [ParentStyle](#parentstyle) | Style | Gets the parent style of this style. |
| [IsNumberFormatApplied](#isnumberformatapplied) | boolean | Indicate whether the number formatting should be applied. Only for named style. |
| [IsFontApplied](#isfontapplied) | boolean | Indicate whether the font formatting should be applied. Only for named style. |
| [IsAlignmentApplied](#isalignmentapplied) | boolean | Indicate whether the alignment formatting should be applied. Only for named style. |
| [IsBorderApplied](#isborderapplied) | boolean | Indicate whether the border formatting should be applied. Only for named style. |
| [IsFillApplied](#isfillapplied) | boolean | Indicate whether the fill formatting should be applied. Only for named style. |
| [IsProtectionApplied](#isprotectionapplied) | boolean | Indicate whether the protection formatting should be applied. Only for named style. |
| [IndentLevel](#indentlevel) | Number | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment ty |
| [Font](#font) | Font | Gets a Font object. |
| [RotationAngle](#rotationangle) | Number | Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. You can set 255 or value  |
| [HorizontalAlignment](#horizontalalignment) | Number | Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer |
| [VerticalAlignment](#verticalalignment) | Number | Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer c |
| [IsTextWrapped](#istextwrapped) | boolean | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [Number](#number) | Number | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For e |
| [IsLocked](#islocked) | boolean | Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet  |
| [Custom](#custom) | String | Represents the custom number format string of this style object. If the custom number format is not set(For example, the |
| [CultureCustom](#culturecustom) | String | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object,  |
| [InvariantCustom](#invariantcustom) | String | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null wi |
| [IsFormulaHidden](#isformulahidden) | boolean | Represents if the formula will be hidden when the worksheet is protected. |
| [ShrinkToFit](#shrinktofit) | boolean | Represents if text automatically shrinks to fit in the available column width. |
| [TextDirection](#textdirection) | Number | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [IsJustifyDistributed](#isjustifydistributed) | boolean | Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for E |
| [QuotePrefix](#quoteprefix) | boolean | Indicates whether the cell's value starts with single quote mark. |
| [IsGradient](#isgradient) | boolean | Indicates whether the cell shading is a gradient pattern. |
| [IsPercent](#ispercent) | boolean | Indicates whether the number format is a percent format. |
| [IsDateTime](#isdatetime) | boolean | Indicates whether the number format is a date format. |
| [IsCheckBox](#ischeckbox) | boolean |  |
| [LeftBorder](#leftborder) | Border |  |
| [RightBorder](#rightborder) | Border |  |
| [TopBorder](#topborder) | Border |  |
| [BottomBorder](#bottomborder) | Border |  |

## Methods

| Name | Description |
| --- | --- |
| [setTwoColorGradient](#settwocolorgradient) | Sets the specified fill to a two-color gradient. |
| [getTwoColorGradient](#gettwocolorgradient) | Get the two-color gradient setting.

If this is not gradient fill,return null; |
| [getTwoColorGradientSetting](#gettwocolorgradientsetting) | Get the two-color gradient setting. |
| [toJson](#tojson) | Convert Style to JSON struct data. |
| [setPatternColor](#setpatterncolor) | Sets the background color. |
| [copy](#copy) | Copies data from another style object

This method does not copy the name of the style. If you want to copy the name, pl |
| [update](#update) | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button afte |
| [isModified](#ismodified) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to che |
| [equals](#equals) | Determines whether two Style instances are equal. |
| [hashCode](#hashcode) | Serves as a hash function for a Style object.

This method is only for internal use. |
| [setBorder](#setborder) | Sets the borders of the style. |
| [setCustom](#setcustom) | Sets the Custom number format string of a cell. |

### Style() {#constructor}

Initializes a new instance of the Style class. NOTE: This constructor is now obsolete. Instead, please use CellsFactory.CreateStyle() method. This property will be removed 6 months later since October 2016. Aspose apologizes for any inconvenience you may have experienced.

### Style.BackgroundThemeColor property {#backgroundthemecolor}

Gets and sets the background theme color. If the background color is not a theme color, NULL will be returned.

**Type:** ThemeColor

### Style.ForegroundThemeColor property {#foregroundthemecolor}

Gets and sets the foreground theme color. If the foreground color is not a theme color, NULL will be returned.

**Type:** ThemeColor

### Style.Name property {#name}

Gets or sets the name of the style.

**Type:** String

### Style.Pattern property {#pattern}

Gets or sets the cell background pattern type. The value of the property is BackgroundType integer constant.

**Type:** Number

### Style.Borders property {#borders}

Gets the BorderCollection of the style.

**Type:** BorderCollection

### Style.BackgroundColor property {#backgroundcolor}

Gets or sets a style's background color. If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

**Type:** Color

### Style.BackgroundArgbColor property {#backgroundargbcolor}

Gets and sets the background color with a 32-bit ARGB value.

**Type:** Number

### Style.ForegroundColor property {#foregroundcolor}

Gets or sets a style's foreground color. It means no color setting if Color.Empty is returned.

**Type:** Color

### Style.ForegroundArgbColor property {#foregroundargbcolor}

Gets and sets the foreground color with a 32-bit ARGB value.

**Type:** Number

### Style.HasBorders property {#hasborders}

Checks whether there are borders have been set for the style.

**Type:** boolean

### Style.ParentStyle property {#parentstyle}

Gets the parent style of this style.

**Type:** Style

### Style.IsNumberFormatApplied property {#isnumberformatapplied}

Indicate whether the number formatting should be applied. Only for named style.

**Type:** boolean

### Style.IsFontApplied property {#isfontapplied}

Indicate whether the font formatting should be applied. Only for named style.

**Type:** boolean

### Style.IsAlignmentApplied property {#isalignmentapplied}

Indicate whether the alignment formatting should be applied. Only for named style.

**Type:** boolean

### Style.IsBorderApplied property {#isborderapplied}

Indicate whether the border formatting should be applied. Only for named style.

**Type:** boolean

### Style.IsFillApplied property {#isfillapplied}

Indicate whether the fill formatting should be applied. Only for named style.

**Type:** boolean

### Style.IsProtectionApplied property {#isprotectionapplied}

Indicate whether the protection formatting should be applied. Only for named style.

**Type:** boolean

### Style.IndentLevel property {#indentlevel}

Represents the indent level for the cell or range. Can only be an integer from 0 to 250. If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

**Type:** Number

### Style.Font property {#font}

Gets a Font object.

**Type:** Font

### Style.RotationAngle property {#rotationangle}

Represents text rotation angle. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. You can set 255 or value ranged from -90 to 90.

**Type:** Number

### Style.HorizontalAlignment property {#horizontalalignment}

Gets or sets the horizontal alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### Style.VerticalAlignment property {#verticalalignment}

Gets or sets the vertical alignment type of the text in a cell. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### Style.IsTextWrapped property {#istextwrapped}

Gets or sets a value indicating whether the text within a cell is wrapped.

**Type:** boolean

### Style.Number property {#number}

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. For example, the formatting patterns represented by numbers for en_US region: Value Type Format String 0 General General 1 Decimal 0 2 Decimal 0.00 3 Decimal #,##0 4 Decimal #,##0.00 5 Currency $#,##0_);($#,##0) 6 Currency $#,##0_);[Red]($#,##0) 7 Currency $#,##0.00_);($#,##0.00) 8 Currency $#,##0.00_);[Red]($#,##0.00) 9 Percentage 0% 10 Percentage 0.00% 11 Scientific 0.00E+00 12 Fraction # ?/? 13 Fraction # ??/?? 14 Date m/d/yyyy 15 Date d-mmm-yy 16 Date d-mmm 17 Date mmm-yy 18 Time h:mm AM/PM 19 Time h:mm:ss AM/PM 20 Time h:mm 21 Time h:mm:ss 22 Time m/d/yyyy h:mm 37 Accounting #,##0_);(#,##0) 38 Accounting #,##0_);[Red](#,##0) 39 Accounting #,##0.00_);(#,##0.00) 40 Accounting #,##0.00_);[Red](#,##0.00) 41 Accounting _(* #,##0_);_(* (#,##0);_(* "-"_);_(@_) 42 Currency _($* #,##0_);_($* (#,##0);_($* "-"_);_(@_) 43 Accounting _(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_) 44 Currency _($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_) 45 Time mm:ss 46 Time [h]:mm:ss 47 Time mm:ss.0 48 Scientific ##0.0E+0 49 Text @

**Type:** Number

### Style.IsLocked property {#islocked}

Gets or sets a value indicating whether a cell can be modified or not. Locking cells has no effect unless the worksheet is protected.

**Type:** boolean

### Style.Custom property {#custom}

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. The returned custom string is culture-independent.

**Type:** String

### Style.CultureCustom property {#culturecustom}

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

**Type:** String

### Style.InvariantCustom property {#invariantcustom}

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from CultureCustom is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.

**Type:** String

### Style.IsFormulaHidden property {#isformulahidden}

Represents if the formula will be hidden when the worksheet is protected.

**Type:** boolean

### Style.ShrinkToFit property {#shrinktofit}

Represents if text automatically shrinks to fit in the available column width.

**Type:** boolean

### Style.TextDirection property {#textdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant.

**Type:** Number

### Style.IsJustifyDistributed property {#isjustifydistributed}

Indicates if the cells justified or distributed alignment should be used on the last line of text. This is typical for East Asian alignments but not typical in other contexts.

**Type:** boolean

### Style.QuotePrefix property {#quoteprefix}

Indicates whether the cell's value starts with single quote mark.

**Type:** boolean

### Style.IsGradient property {#isgradient}

Indicates whether the cell shading is a gradient pattern.

**Type:** boolean

### Style.IsPercent property {#ispercent}

Indicates whether the number format is a percent format.

**Type:** boolean

### Style.IsDateTime property {#isdatetime}

Indicates whether the number format is a date format.

**Type:** boolean

### Style.IsCheckBox property {#ischeckbox}

**Type:** boolean

### Style.LeftBorder property {#leftborder}

**Type:** Border

### Style.RightBorder property {#rightborder}

**Type:** Border

### Style.TopBorder property {#topborder}

**Type:** Border

### Style.BottomBorder property {#bottomborder}

**Type:** Border

### setTwoColorGradient(color1, color2, gradientStyleType, variant) {#settwocolorgradient}

Sets the specified fill to a two-color gradient.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| gradientStyleType | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### getTwoColorGradient() {#gettwocolorgradient}

Get the two-color gradient setting.

If this is not gradient fill,return null;

**Returns:** Returns all setting about two-color gradient [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant

### getTwoColorGradientSetting() {#gettwocolorgradientsetting}

Get the two-color gradient setting.

### toJson() {#tojson}

Convert Style to JSON struct data.

### setPatternColor(pattern, color1, color2) {#setpatterncolor}

Sets the background color.

| Parameter | Type | Description |
| --- | --- | --- |
| pattern | Number | A BackgroundType value. The pattern. |
| color1 | Color | The foreground color. |
| color2 | Color | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |

### copy(style) {#copy}

Copies data from another style object

This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |

### update() {#update}

Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.

### isModified(modifyFlag) {#ismodified}

Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | Number | A StyleModifyFlag value. Style modified flags |

**Returns:** true if the specified properties have been modified

### equals(obj) {#equals}

Determines whether two Style instances are equal.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The Style object to compare with the current Style object. |

**Returns:** true if the specified Object is equal to the current Object; otherwise, false.

### hashCode() {#hashcode}

Serves as a hash function for a Style object.

This method is only for internal use.

**Returns:** A hash code for the current Object.

### setBorder(borderType, borderStyle, borderColor) (1 of 2) {#setborder}

Sets the borders of the style.

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | Number | A BorderType value. The border(s) to be set, can be combination of BorderType . |
| borderStyle | Number | A CellBorderType value. The style of the border. |
| borderColor | Color | The color of the border. |

**Returns:** Whether current border settings have been changed.

---

### setBorder(borderType, borderStyle, borderColor) (2 of 2) {#setborder-1}

Sets the borders of the style.

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | Number | A BorderType value. The border(s) to be set, can be combination of BorderType . |
| borderStyle | Number | A CellBorderType value. The style of the border. |
| borderColor | CellsColor | The color of the border. |

**Returns:** Whether current border settings have been changed.

### setCustom(custom, builtinPreference) {#setcustom}

Sets the Custom number format string of a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| custom | String | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | boolean | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |
