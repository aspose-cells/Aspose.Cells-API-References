##Style
Represents display style of excel documentsuch as fontcoloralignmentborderetc.
**Inheritance:**
java.lang.Object
```
public class Style
```
Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties.
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
## Constructors
| Constructor | Description |
| --- | --- |
| [Style()](#Style--) | Initializes a new instance of the [Style](../../com.aspose.cells/style) class. |
## Methods
| Method | Description |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Copies data from another style object |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether two Style instances are equal. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Gets the background color with a 32-bit ARGB value. |
| [getBackgroundColor()](#getBackgroundColor--) | Gets a style's background color. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Gets the background theme color. |
| [getBorders()](#getBorders--) | Gets the [BorderCollection](../../com.aspose.cells/bordercollection) of the style. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Gets the culture-dependent pattern string for number format. |
| [getCustom()](#getCustom--) | Represents the custom number format string of this style object. |
| [getFont()](#getFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object. |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Gets the foreground color with a 32-bit ARGB value. |
| [getForegroundColor()](#getForegroundColor--) | Gets a style's foreground color. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Gets the foreground theme color. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Gets the horizontal alignment type of the text in a cell. |
| [getIndentLevel()](#getIndentLevel--) | Represents the indent level for the cell or range. |
| [getInvariantCustom()](#getInvariantCustom--) | Gets the culture-independent pattern string for number format. |
| [getName()](#getName--) | Gets the name of the style. |
| [getNumber()](#getNumber--) | Gets the display format of numbers and dates. |
| [getParentStyle()](#getParentStyle--) | Gets the parent style of this style. |
| [getPattern()](#getPattern--) | Gets the cell background pattern type. |
| [getQuotePrefix()](#getQuotePrefix--) | Indicates whether the cell's value starts with single quote mark. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle. |
| [getShrinkToFit()](#getShrinkToFit--) | Represents if text automatically shrinks to fit in the available column width. |
| [getTextDirection()](#getTextDirection--) | Represents text reading order. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Get the two-color gradient setting. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Get the two-color gradient setting. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Gets the vertical alignment type of the text in a cell. |
| [hasBorders()](#hasBorders--) | Checks whether there are borders have been set for the style. |
| [hashCode()](#hashCode--) | Serves as a hash function for a Style object. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Indicate whether the alignment formatting should be applied. |
| [isBorderApplied()](#isBorderApplied--) | Indicate whether the border formatting should be applied. |
| [isDateTime()](#isDateTime--) | Indicates whether the number format is a date format. |
| [isFillApplied()](#isFillApplied--) | Indicate whether the fill formatting should be applied. |
| [isFontApplied()](#isFontApplied--) | Indicate whether the font formatting should be applied. |
| [isFormulaHidden()](#isFormulaHidden--) | Represents if the formula will be hidden when the worksheet is protected. |
| [isGradient()](#isGradient--) | Indicates whether the cell shading is a gradient pattern. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [isLocked()](#isLocked--) | Gets a value indicating whether a cell can be modified or not. |
| [isModified(int modifyFlag)](#isModified-int-) | Checks whether the specified properties of the style have been modified. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Indicate whether the number formatting should be applied. |
| [isPercent()](#isPercent--) | Indicates whether the number format is a percent format. |
| [isProtectionApplied()](#isProtectionApplied--) | Indicate whether the protection formatting should be applied. |
| [isTextWrapped()](#isTextWrapped--) | Gets a value indicating whether the text within a cell is wrapped. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Indicate whether the alignment formatting should be applied. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Sets the background color with a 32-bit ARGB value. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Sets a style's background color. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Sets the background theme color. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Sets the borders of the style. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Sets the borders of the style. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Indicate whether the border formatting should be applied. |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Sets the culture-dependent pattern string for number format. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Represents the custom number format string of this style object. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Sets the Custom number format string of a cell. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Indicate whether the fill formatting should be applied. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Indicate whether the font formatting should be applied. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Sets the foreground color with a 32-bit ARGB value. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Sets a style's foreground color. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Sets the foreground theme color. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Represents if the formula will be hidden when the worksheet is protected. |
| [setGradient(boolean value)](#setGradient-boolean-) | Indicates whether the cell shading is a gradient pattern. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Sets the horizontal alignment type of the text in a cell. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Represents the indent level for the cell or range. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [setLocked(boolean value)](#setLocked-boolean-) | Sets a value indicating whether a cell can be modified or not. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the style. |
| [setNumber(int value)](#setNumber-int-) | Sets the display format of numbers and dates. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Indicate whether the number formatting should be applied. |
| [setPattern(int value)](#setPattern-int-) | Sets the cell background pattern type. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Sets the background color. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Indicate whether the protection formatting should be applied. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indicates whether the cell's value starts with single quote mark. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents text rotation angle. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Represents if text automatically shrinks to fit in the available column width. |
| [setTextDirection(int value)](#setTextDirection-int-) | Represents text reading order. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets a value indicating whether the text within a cell is wrapped. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Sets the specified fill to a two-color gradient. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Sets the vertical alignment type of the text in a cell. |
| [toJson()](#toJson--) | Convert [Style](../../com.aspose.cells/style) to JSON struct data. |
| [toString()](#toString--) |  |
| [update()](#update--) | Apply the named style to the styles of the cells which use this named style. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```
Initializes a new instance of the [Style](../../com.aspose.cells/style) class.
**Remarks**
NOTE: This constructor is now obsolete. Instead, please use CellsFactory.CreateStyle() method. This property will be removed 6 months later since October 2016. Aspose apologizes for any inconvenience you may have experienced.
### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```
Copies data from another style object
**Remarks**
This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Source Style object |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Determines whether two Style instances are equal.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The Style object to compare with the current Style object. |
**Returns:**
boolean - true if the specified Object is equal to the current Object; otherwise, false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```
Gets the background color with a 32-bit ARGB value.
**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```
Gets a style's background color.
**Remarks**
If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.
**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```
Gets the background theme color.
**Remarks**
If the background color is not a theme color, NULL will be returned.
**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```
Gets the [BorderCollection](../../com.aspose.cells/bordercollection) of the style.
**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
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
Gets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.
**Remarks**
For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.
**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```
Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.
**Remarks**
The returned custom string is culture-independent.
**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```
Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object.
**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```
Gets the foreground color with a 32-bit ARGB value.
**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```
Gets a style's foreground color.
**Remarks**
It means no color setting if Color.Empty is returned.
**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```
Gets the foreground theme color.
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```
Gets the horizontal alignment type of the text in a cell.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```
Represents the indent level for the cell or range. Can only be an integer from 0 to 250.
**Remarks**
If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.
**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```
Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.
**Remarks**
For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.
**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```
Gets the name of the style.
**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```
Gets the display format of numbers and dates. The formatting patterns are different for different regions.
**Remarks**
For example, the formatting patterns represented by numbers for en\_US region:
| Value | Type       | Format String                                        |
| ----- | ---------- | ---------------------------------------------------- |
| 0     | General    | `General`                                            |
| 1     | Decimal    | `0`                                                  |
| 2     | Decimal    | `0.00`                                               |
| 3     | Decimal    | `#,##0`                                              |
| 4     | Decimal    | `#,##0.00`                                           |
| 5     | Currency   | `$#,##0_);($#,##0)`                                  |
| 6     | Currency   | `$#,##0_);[Red](../$#,##0)`                             |
| 7     | Currency   | `$#,##0.00_);($#,##0.00)`                            |
| 8     | Currency   | `$#,##0.00_);[Red](../$#,##0.00)`                       |
| 9     | Percentage | `0%`                                                 |
| 10    | Percentage | `0.00%`                                              |
| 11    | Scientific | `0.00E+00`                                           |
| 12    | Fraction   | `# ?/?`                                              |
| 13    | Fraction   | `# ??/??`                                            |
| 14    | Date       | `m/d/yyyy`                                           |
| 15    | Date       | `d-mmm-yy`                                           |
| 16    | Date       | `d-mmm`                                              |
| 17    | Date       | `mmm-yy`                                             |
| 18    | Time       | `h:mm AM/PM`                                         |
| 19    | Time       | `h:mm:ss AM/PM`                                      |
| 20    | Time       | `h:mm`                                               |
| 21    | Time       | `h:mm:ss`                                            |
| 22    | Time       | `m/d/yyyy h:mm`                                      |
| 37    | Accounting | `#,##0_);(#,##0)`                                    |
| 38    | Accounting | `#,##0_);[Red](../#,##0)`                               |
| 39    | Accounting | `#,##0.00_);(#,##0.00)`                              |
| 40    | Accounting | `#,##0.00_);[Red](../#,##0.00)`                         |
| 41    | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)`            |
| 42    | Currency   | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)`         |
| 43    | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)`    |
| 44    | Currency   | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45    | Time       | `mm:ss`                                              |
| 46    | Time       | `[h]:mm:ss`                                          |
| 47    | Time       | `mm:ss.0`                                            |
| 48    | Scientific | `##0.0E+0`                                           |
| 49    | Text       | `@`                                                  |
**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```
Gets the parent style of this style.
**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```
Gets the cell background pattern type.
See [BackgroundType](../../com.aspose.cells/backgroundtype).
**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```
Indicates whether the cell's value starts with single quote mark.
**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```
Represents text rotation angle.
**Remarks**
0: Not rotated.
255: Top to Bottom.
\-90: Downward.
90: Upward.
You can set 255 or value ranged from -90 to 90.
**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```
Represents if text automatically shrinks to fit in the available column width.
**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Returns:**
int
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```
Get the two-color gradient setting.
**Remarks**
NOTE: This method is now obsolete. Instead, please use Style.GetTwoColorGradientSetting() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
java.lang.Object[] - Returns all setting about two-color gradient [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```
Get the two-color gradient setting.
**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```
Gets the vertical alignment type of the text in a cell.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```
Checks whether there are borders have been set for the style.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```
Serves as a hash function for a Style object.
**Remarks**
This method is only for internal use.
**Returns:**
int - A hash code for the current Object.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```
Indicate whether the alignment formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```
Indicate whether the border formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```
Indicates whether the number format is a date format.
**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```
Indicate whether the fill formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```
Indicate whether the font formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```
Represents if the formula will be hidden when the worksheet is protected.
**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```
Indicates whether the cell shading is a gradient pattern.
**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```
Indicates if the cells justified or distributed alignment should be used on the last line of text.
**Remarks**
This is typical for East Asian alignments but not typical in other contexts.
**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```
Gets a value indicating whether a cell can be modified or not.
**Remarks**
Locking cells has no effect unless the worksheet is protected.
**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```
Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Style modified flags |
**Returns:**
boolean - true if the specified properties have been modified
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```
Indicate whether the number formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```
Indicates whether the number format is a percent format.
**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```
Indicate whether the protection formatting should be applied.
**Remarks**
Only for named style.
**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```
Gets a value indicating whether the text within a cell is wrapped.
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
Indicate whether the alignment formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```
Sets the background color with a 32-bit ARGB value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```
Sets a style's background color.
**Remarks**
If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```
Sets the background theme color.
**Remarks**
If the background color is not a theme color, NULL will be returned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |
### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```
Sets the borders of the style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). The border(s) to be set, can be combination of [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). The style of the border. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | The color of the border. |
**Returns:**
boolean - Whether current border settings have been changed.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```
Sets the borders of the style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). The border(s) to be set, can be combination of [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). The style of the border. |
| borderColor | [Color](../../com.aspose.cells/color) | The color of the border. |
**Returns:**
boolean - Whether current border settings have been changed.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```
Indicate whether the border formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```
Sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.
**Remarks**
For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```
Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.
**Remarks**
The returned custom string is culture-independent.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```
Sets the Custom number format string of a cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| custom | java.lang.String | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | boolean | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |
### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```
Indicate whether the fill formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```
Indicate whether the font formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```
Sets the foreground color with a 32-bit ARGB value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```
Sets a style's foreground color.
**Remarks**
It means no color setting if Color.Empty is returned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```
Sets the foreground theme color.
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |
### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```
Represents if the formula will be hidden when the worksheet is protected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```
Indicates whether the cell shading is a gradient pattern.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```
Sets the horizontal alignment type of the text in a cell.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```
Represents the indent level for the cell or range. Can only be an integer from 0 to 250.
**Remarks**
If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```
Indicates if the cells justified or distributed alignment should be used on the last line of text.
**Remarks**
This is typical for East Asian alignments but not typical in other contexts.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```
Sets a value indicating whether a cell can be modified or not.
**Remarks**
Locking cells has no effect unless the worksheet is protected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```
Sets the display format of numbers and dates. The formatting patterns are different for different regions.
**Remarks**
For example, the formatting patterns represented by numbers for en\_US region:
| Value | Type       | Format String                                        |
| ----- | ---------- | ---------------------------------------------------- |
| 0     | General    | `General`                                            |
| 1     | Decimal    | `0`                                                  |
| 2     | Decimal    | `0.00`                                               |
| 3     | Decimal    | `#,##0`                                              |
| 4     | Decimal    | `#,##0.00`                                           |
| 5     | Currency   | `$#,##0_);($#,##0)`                                  |
| 6     | Currency   | `$#,##0_);[Red](../$#,##0)`                             |
| 7     | Currency   | `$#,##0.00_);($#,##0.00)`                            |
| 8     | Currency   | `$#,##0.00_);[Red](../$#,##0.00)`                       |
| 9     | Percentage | `0%`                                                 |
| 10    | Percentage | `0.00%`                                              |
| 11    | Scientific | `0.00E+00`                                           |
| 12    | Fraction   | `# ?/?`                                              |
| 13    | Fraction   | `# ??/??`                                            |
| 14    | Date       | `m/d/yyyy`                                           |
| 15    | Date       | `d-mmm-yy`                                           |
| 16    | Date       | `d-mmm`                                              |
| 17    | Date       | `mmm-yy`                                             |
| 18    | Time       | `h:mm AM/PM`                                         |
| 19    | Time       | `h:mm:ss AM/PM`                                      |
| 20    | Time       | `h:mm`                                               |
| 21    | Time       | `h:mm:ss`                                            |
| 22    | Time       | `m/d/yyyy h:mm`                                      |
| 37    | Accounting | `#,##0_);(#,##0)`                                    |
| 38    | Accounting | `#,##0_);[Red](../#,##0)`                               |
| 39    | Accounting | `#,##0.00_);(#,##0.00)`                              |
| 40    | Accounting | `#,##0.00_);[Red](../#,##0.00)`                         |
| 41    | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)`            |
| 42    | Currency   | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)`         |
| 43    | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)`    |
| 44    | Currency   | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45    | Time       | `mm:ss`                                              |
| 46    | Time       | `[h]:mm:ss`                                          |
| 47    | Time       | `mm:ss.0`                                            |
| 48    | Scientific | `##0.0E+0`                                           |
| 49    | Text       | `@`                                                  |
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```
Indicate whether the number formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```
Sets the cell background pattern type.
See [BackgroundType](../../com.aspose.cells/backgroundtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```
Sets the background color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). The pattern. |
| color1 | [Color](../../com.aspose.cells/color) | The foreground color. |
| color2 | [Color](../../com.aspose.cells/color) | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |
### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```
Indicate whether the protection formatting should be applied.
**Remarks**
Only for named style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```
Indicates whether the cell's value starts with single quote mark.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```
Represents text rotation angle.
**Remarks**
0: Not rotated.
255: Top to Bottom.
\-90: Downward.
90: Upward.
You can set 255 or value ranged from -90 to 90.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```
Represents if text automatically shrinks to fit in the available column width.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```
Sets a value indicating whether the text within a cell is wrapped.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```
Sets the specified fill to a two-color gradient.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | One gradient color. |
| color2 | [Color](../../com.aspose.cells/color) | Two gradient color. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```
Sets the vertical alignment type of the text in a cell.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### toJson() {#toJson--}
```
public String toJson()
```
Convert [Style](../../com.aspose.cells/style) to JSON struct data.
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
Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
