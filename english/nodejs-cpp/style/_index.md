---
title: Style
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents display style of excel documentsuch as fontcoloralignmentborderetc. The Style object contains all style attributes font number format alignment and so on as properties.
type: docs
url: /nodejs-cpp/style/
---

## Style class

Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties.

```javascript
class Style;
```


### Example
```javascript
//First method
const { Workbook, Color } = require("aspose.cells.node");

var excel = new Workbook();
var style = excel.createStyle();
style.getFont().setName("Times New Roman");
style.getFont().setColor(Color.Blue);
for (var i = 0; i < 100; i++) {
    excel.getWorksheets().get(0).getCells().get(0, i).setStyle(style);
}

//Second method
var style1 = excel.getWorksheets().get(0).getCells().get("A1").getStyle();
style1.getFont().setName("Times New Roman");
style1.getFont().setColor(Color.Blue);
excel.getWorksheets().get(0).getCells().get("A1").setStyle(style1);

//First method is a fast and efficient way to change several cell-formatting properties on multiple cells at the same time.
//If you want to change a single cell's style properties, second method can be used.
```
## Methods

| Method | Description |
| --- | --- |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--)| Gets and sets the background theme color. |
| [setBackgroundThemeColor(ThemeColor)](#setBackgroundThemeColor-themecolor-)| Gets and sets the background theme color. |
| [getForegroundThemeColor()](#getForegroundThemeColor--)| Gets and sets the foreground theme color. |
| [setForegroundThemeColor(ThemeColor)](#setForegroundThemeColor-themecolor-)| Gets and sets the foreground theme color. |
| [getName()](#getName--)| Gets or sets the name of the style. |
| [setName(string)](#setName-string-)| Gets or sets the name of the style. |
| [getPattern()](#getPattern--)| Gets or sets the cell background pattern type. |
| [setPattern(BackgroundType)](#setPattern-backgroundtype-)| Gets or sets the cell background pattern type. |
| [getBorders()](#getBorders--)| Gets the [BorderCollection](../bordercollection/) of the style. |
| [getBackgroundColor()](#getBackgroundColor--)| Gets or sets a style's background color. |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| Gets or sets a style's background color. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--)| Gets and sets the background color with a 32-bit ARGB value. |
| [setBackgroundArgbColor(number)](#setBackgroundArgbColor-number-)| Gets and sets the background color with a 32-bit ARGB value. |
| [getForegroundColor()](#getForegroundColor--)| Gets or sets a style's foreground color. |
| [setForegroundColor(Color)](#setForegroundColor-color-)| Gets or sets a style's foreground color. |
| [getForegroundArgbColor()](#getForegroundArgbColor--)| Gets and sets the foreground color with a 32-bit ARGB value. |
| [setForegroundArgbColor(number)](#setForegroundArgbColor-number-)| Gets and sets the foreground color with a 32-bit ARGB value. |
| [getHasBorders()](#getHasBorders--)| Checks whether there are borders have been set for the style. |
| [getParentStyle()](#getParentStyle--)| Gets the parent style of this style. |
| [isNumberFormatApplied()](#isNumberFormatApplied--)| Indicate whether the number formatting should be applied. |
| [setIsNumberFormatApplied(boolean)](#setIsNumberFormatApplied-boolean-)| Indicate whether the number formatting should be applied. |
| [isFontApplied()](#isFontApplied--)| Indicate whether the font formatting should be applied. |
| [setIsFontApplied(boolean)](#setIsFontApplied-boolean-)| Indicate whether the font formatting should be applied. |
| [isAlignmentApplied()](#isAlignmentApplied--)| Indicate whether the alignment formatting should be applied. |
| [setIsAlignmentApplied(boolean)](#setIsAlignmentApplied-boolean-)| Indicate whether the alignment formatting should be applied. |
| [isBorderApplied()](#isBorderApplied--)| Indicate whether the border formatting should be applied. |
| [setIsBorderApplied(boolean)](#setIsBorderApplied-boolean-)| Indicate whether the border formatting should be applied. |
| [isFillApplied()](#isFillApplied--)| Indicate whether the fill formatting should be applied. |
| [setIsFillApplied(boolean)](#setIsFillApplied-boolean-)| Indicate whether the fill formatting should be applied. |
| [isProtectionApplied()](#isProtectionApplied--)| Indicate whether the protection formatting should be applied. |
| [setIsProtectionApplied(boolean)](#setIsProtectionApplied-boolean-)| Indicate whether the protection formatting should be applied. |
| [getIndentLevel()](#getIndentLevel--)| Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [setIndentLevel(number)](#setIndentLevel-number-)| Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object. |
| [getRotationAngle()](#getRotationAngle--)| Represents text rotation angle. |
| [setRotationAngle(number)](#setRotationAngle-number-)| Represents text rotation angle. |
| [getHorizontalAlignment()](#getHorizontalAlignment--)| Gets or sets the horizontal alignment type of the text in a cell. |
| [setHorizontalAlignment(TextAlignmentType)](#setHorizontalAlignment-textalignmenttype-)| Gets or sets the horizontal alignment type of the text in a cell. |
| [getVerticalAlignment()](#getVerticalAlignment--)| Gets or sets the vertical alignment type of the text in a cell. |
| [setVerticalAlignment(TextAlignmentType)](#setVerticalAlignment-textalignmenttype-)| Gets or sets the vertical alignment type of the text in a cell. |
| [isTextWrapped()](#isTextWrapped--)| Gets or sets a value indicating whether the text within a cell is wrapped. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| Gets or sets a value indicating whether the text within a cell is wrapped. |
| [getNumber()](#getNumber--)| Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [setNumber(number)](#setNumber-number-)| Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [isLocked()](#isLocked--)| Gets or sets a value indicating whether a cell can be modified or not. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| Gets or sets a value indicating whether a cell can be modified or not. |
| [getCustom()](#getCustom--)| Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [setCustom(string)](#setCustom-string-)| Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [getCultureCustom()](#getCultureCustom--)| Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [setCultureCustom(string)](#setCultureCustom-string-)| Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [getInvariantCustom()](#getInvariantCustom--)| Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [isFormulaHidden()](#isFormulaHidden--)| Represents if the formula will be hidden when the worksheet is protected. |
| [setIsFormulaHidden(boolean)](#setIsFormulaHidden-boolean-)| Represents if the formula will be hidden when the worksheet is protected. |
| [getShrinkToFit()](#getShrinkToFit--)| Represents if text automatically shrinks to fit in the available column width. |
| [setShrinkToFit(boolean)](#setShrinkToFit-boolean-)| Represents if text automatically shrinks to fit in the available column width. |
| [getTextDirection()](#getTextDirection--)| Represents text reading order. |
| [setTextDirection(TextDirectionType)](#setTextDirection-textdirectiontype-)| Represents text reading order. |
| [isJustifyDistributed()](#isJustifyDistributed--)| Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [setIsJustifyDistributed(boolean)](#setIsJustifyDistributed-boolean-)| Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [getQuotePrefix()](#getQuotePrefix--)| Indicates whether the cell's value starts with single quote mark. |
| [setQuotePrefix(boolean)](#setQuotePrefix-boolean-)| Indicates whether the cell's value starts with single quote mark. |
| [isGradient()](#isGradient--)| Indicates whether the cell shading is a gradient pattern. |
| [setIsGradient(boolean)](#setIsGradient-boolean-)| Indicates whether the cell shading is a gradient pattern. |
| [isPercent()](#isPercent--)| Indicates whether the number format is a percent format. |
| [isDateTime()](#isDateTime--)| Indicates whether the number format is a date format. |
| [setPatternColor(BackgroundType, Color, Color)](#setPatternColor-backgroundtype-color-color-)| Sets the background color. |
| [copy(Style)](#copy-style-)| Copies data from another style object |
| [update()](#update--)| Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style. |
| [isModified(StyleModifyFlag)](#isModified-stylemodifyflag-)| Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell. |
| [equals(Object)](#equals-object-)| Determines whether two Style instances are equal. |
| [getHashCode()](#getHashCode--)| Serves as a hash function for a Style object. |
| [setBorder(BorderType, CellBorderType, Color)](#setBorder-bordertype-cellbordertype-color-)| Sets the borders of the style. |
| [setBorder(BorderType, CellBorderType, CellsColor)](#setBorder-bordertype-cellbordertype-cellscolor-)| Sets the borders of the style. |
| [setCustom(string, boolean)](#setCustom-string-boolean-)| Sets the Custom number format string of a cell. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--)| Get the two-color gradient setting. |
| [toJson()](#toJson--)| Convert [Style](../style/) to JSON struct data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getBackgroundThemeColor() {#getBackgroundThemeColor--}

Gets and sets the background theme color.

```javascript
getBackgroundThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

**Remarks**

If the background color is not a theme color, NULL will be returned.

### setBackgroundThemeColor(ThemeColor) {#setBackgroundThemeColor-themecolor-}

Gets and sets the background theme color.

```javascript
setBackgroundThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

**Remarks**

If the background color is not a theme color, NULL will be returned.

### getForegroundThemeColor() {#getForegroundThemeColor--}

Gets and sets the foreground theme color.

```javascript
getForegroundThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

**Remarks**

If the foreground color is not a theme color, NULL will be returned.

### setForegroundThemeColor(ThemeColor) {#setForegroundThemeColor-themecolor-}

Gets and sets the foreground theme color.

```javascript
setForegroundThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

**Remarks**

If the foreground color is not a theme color, NULL will be returned.

### getName() {#getName--}

Gets or sets the name of the style.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets or sets the name of the style.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPattern() {#getPattern--}

Gets or sets the cell background pattern type.

```javascript
getPattern() : BackgroundType;
```


**Returns**

[BackgroundType](../backgroundtype/)

### setPattern(BackgroundType) {#setPattern-backgroundtype-}

Gets or sets the cell background pattern type.

```javascript
setPattern(value: BackgroundType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundType](../backgroundtype/) | The value to set. |

### getBorders() {#getBorders--}

Gets the [BorderCollection](../bordercollection/) of the style.

```javascript
getBorders() : BorderCollection;
```


**Returns**

[BorderCollection](../bordercollection/)

### getBackgroundColor() {#getBackgroundColor--}

Gets or sets a style's background color.

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### setBackgroundColor(Color) {#setBackgroundColor-color-}

Gets or sets a style's background color.

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

**Remarks**

If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### getBackgroundArgbColor() {#getBackgroundArgbColor--}

Gets and sets the background color with a 32-bit ARGB value.

```javascript
getBackgroundArgbColor() : number;
```


### setBackgroundArgbColor(number) {#setBackgroundArgbColor-number-}

Gets and sets the background color with a 32-bit ARGB value.

```javascript
setBackgroundArgbColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getForegroundColor() {#getForegroundColor--}

Gets or sets a style's foreground color.

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

It means no color setting if Color.Empty is returned.

### setForegroundColor(Color) {#setForegroundColor-color-}

Gets or sets a style's foreground color.

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

**Remarks**

It means no color setting if Color.Empty is returned.

### getForegroundArgbColor() {#getForegroundArgbColor--}

Gets and sets the foreground color with a 32-bit ARGB value.

```javascript
getForegroundArgbColor() : number;
```


### setForegroundArgbColor(number) {#setForegroundArgbColor-number-}

Gets and sets the foreground color with a 32-bit ARGB value.

```javascript
setForegroundArgbColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHasBorders() {#getHasBorders--}

Checks whether there are borders have been set for the style.

```javascript
getHasBorders() : boolean;
```


### getParentStyle() {#getParentStyle--}

Gets the parent style of this style.

```javascript
getParentStyle() : Style;
```


**Returns**

[Style](../style/)

### isNumberFormatApplied() {#isNumberFormatApplied--}

Indicate whether the number formatting should be applied.

```javascript
isNumberFormatApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsNumberFormatApplied(boolean) {#setIsNumberFormatApplied-boolean-}

Indicate whether the number formatting should be applied.

```javascript
setIsNumberFormatApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### isFontApplied() {#isFontApplied--}

Indicate whether the font formatting should be applied.

```javascript
isFontApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsFontApplied(boolean) {#setIsFontApplied-boolean-}

Indicate whether the font formatting should be applied.

```javascript
setIsFontApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### isAlignmentApplied() {#isAlignmentApplied--}

Indicate whether the alignment formatting should be applied.

```javascript
isAlignmentApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsAlignmentApplied(boolean) {#setIsAlignmentApplied-boolean-}

Indicate whether the alignment formatting should be applied.

```javascript
setIsAlignmentApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### isBorderApplied() {#isBorderApplied--}

Indicate whether the border formatting should be applied.

```javascript
isBorderApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsBorderApplied(boolean) {#setIsBorderApplied-boolean-}

Indicate whether the border formatting should be applied.

```javascript
setIsBorderApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### isFillApplied() {#isFillApplied--}

Indicate whether the fill formatting should be applied.

```javascript
isFillApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsFillApplied(boolean) {#setIsFillApplied-boolean-}

Indicate whether the fill formatting should be applied.

```javascript
setIsFillApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### isProtectionApplied() {#isProtectionApplied--}

Indicate whether the protection formatting should be applied.

```javascript
isProtectionApplied() : boolean;
```


**Remarks**

Only for named style.

### setIsProtectionApplied(boolean) {#setIsProtectionApplied-boolean-}

Indicate whether the protection formatting should be applied.

```javascript
setIsProtectionApplied(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for named style.

### getIndentLevel() {#getIndentLevel--}

Represents the indent level for the cell or range. Can only be an integer from 0 to 250.

```javascript
getIndentLevel() : number;
```


**Remarks**

If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### setIndentLevel(number) {#setIndentLevel-number-}

Represents the indent level for the cell or range. Can only be an integer from 0 to 250.

```javascript
setIndentLevel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### getFont() {#getFont--}

Gets a [Font](../font/) object.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getRotationAngle() {#getRotationAngle--}

Represents text rotation angle.

```javascript
getRotationAngle() : number;
```


**Remarks**

0: Not rotated.</p> <p>255: Top to Bottom.</p> <p>-90: Downward.</p> <p>90: Upward.</p> You can set 255 or value ranged from -90 to 90.

### setRotationAngle(number) {#setRotationAngle-number-}

Represents text rotation angle.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

0: Not rotated.</p> <p>255: Top to Bottom.</p> <p>-90: Downward.</p> <p>90: Upward.</p> You can set 255 or value ranged from -90 to 90.

### getHorizontalAlignment() {#getHorizontalAlignment--}

Gets or sets the horizontal alignment type of the text in a cell.

```javascript
getHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setHorizontalAlignment(TextAlignmentType) {#setHorizontalAlignment-textalignmenttype-}

Gets or sets the horizontal alignment type of the text in a cell.

```javascript
setHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getVerticalAlignment() {#getVerticalAlignment--}

Gets or sets the vertical alignment type of the text in a cell.

```javascript
getVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setVerticalAlignment(TextAlignmentType) {#setVerticalAlignment-textalignmenttype-}

Gets or sets the vertical alignment type of the text in a cell.

```javascript
setVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### isTextWrapped() {#isTextWrapped--}

Gets or sets a value indicating whether the text within a cell is wrapped.

```javascript
isTextWrapped() : boolean;
```


### setIsTextWrapped(boolean) {#setIsTextWrapped-boolean-}

Gets or sets a value indicating whether the text within a cell is wrapped.

```javascript
setIsTextWrapped(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNumber() {#getNumber--}

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions.

```javascript
getNumber() : number;
```


**Remarks**

For example, the formatting patterns represented by numbers for en_US region: <list type="table"> <listheader> <description>Value</description> <description>Type</description> <description>Format String</description> </listheader> <item> <description>0</description> <description>General</description> <description><c>General</c></description> </item> <item> <description>1</description> <description>Decimal</description> <description><c>0</c></description> </item> <item> <description>2</description> <description>Decimal</description> <description><c>0.00</c></description> </item> <item> <description>3</description> <description>Decimal</description> <description><c>#,##0</c></description> </item> <item> <description>4</description> <description>Decimal</description> <description><c>#,##0.00</c></description> </item> <item> <description>5</description> <description>Currency</description> <description><c>$#,##0_);($#,##0)</c></description> </item> <item> <description>6</description> <description>Currency</description> <description><c>$#,##0_);[Red]($#,##0)</c></description> </item> <item> <description>7</description> <description>Currency</description> <description><c>$#,##0.00_);($#,##0.00)</c></description> </item> <item> <description>8</description> <description>Currency</description> <description><c>$#,##0.00_);[Red]($#,##0.00)</c></description> </item> <item> <description>9</description> <description>Percentage</description> <description><c>0%</c></description> </item> <item> <description>10</description> <description>Percentage</description> <description><c>0.00%</c></description> </item> <item> <description>11</description> <description>Scientific</description> <description><c>0.00E+00</c></description> </item> <item> <description>12</description> <description>Fraction</description> <description><c># ?/?</c></description> </item> <item> <description>13</description> <description>Fraction</description> <description><c># ??/??</c></description> </item> <item> <description>14</description> <description>Date</description> <description><c>m/d/yyyy</c></description> </item> <item> <description>15</description> <description>Date</description> <description><c>d-mmm-yy</c></description> </item> <item> <description>16</description> <description>Date</description> <description><c>d-mmm</c></description> </item> <item> <description>17</description> <description>Date</description> <description><c>mmm-yy</c></description> </item> <item> <description>18</description> <description>Time</description> <description><c>h:mm AM/PM</c></description> </item> <item> <description>19</description> <description>Time</description> <description><c>h:mm:ss AM/PM</c></description> </item> <item> <description>20</description> <description>Time</description> <description><c>h:mm</c></description> </item> <item> <description>21</description> <description>Time</description> <description><c>h:mm:ss</c></description> </item> <item> <description>22</description> <description>Time</description> <description><c>m/d/yyyy h:mm</c></description> </item> <item> <description>37</description> <description>Accounting</description> <description><c>#,##0_);(#,##0)</c></description> </item> <item> <description>38</description> <description>Accounting</description> <description><c>#,##0_);[Red](#,##0)</c></description> </item> <item> <description>39</description> <description>Accounting</description> <description><c>#,##0.00_);(#,##0.00)</c></description> </item> <item> <description>40</description> <description>Accounting</description> <description><c>#,##0.00_);[Red](#,##0.00)</c></description> </item> <item> <description>41</description> <description>Accounting</description> <description><c>_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)</c></description> </item> <item> <description>42</description> <description>Currency</description> <description><c>_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)</c></description> </item> <item> <description>43</description> <description>Accounting</description> <description><c>_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)</c></description> </item> <item> <description>44</description> <description>Currency</description> <description><c>_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)</c></description> </item> <item> <description>45</description> <description>Time</description> <description><c>mm:ss</c></description> </item> <item> <description>46</description> <description>Time</description> <description><c>[h]:mm:ss</c></description> </item> <item> <description>47</description> <description>Time</description> <description><c>mm:ss.0</c></description> </item> <item> <description>48</description> <description>Scientific</description> <description><c>##0.0E+0</c></description> </item> <item> <description>49</description> <description>Text</description> <description><c>@</c></description> </item> </list

### setNumber(number) {#setNumber-number-}

Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions.

```javascript
setNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

For example, the formatting patterns represented by numbers for en_US region: <list type="table"> <listheader> <description>Value</description> <description>Type</description> <description>Format String</description> </listheader> <item> <description>0</description> <description>General</description> <description><c>General</c></description> </item> <item> <description>1</description> <description>Decimal</description> <description><c>0</c></description> </item> <item> <description>2</description> <description>Decimal</description> <description><c>0.00</c></description> </item> <item> <description>3</description> <description>Decimal</description> <description><c>#,##0</c></description> </item> <item> <description>4</description> <description>Decimal</description> <description><c>#,##0.00</c></description> </item> <item> <description>5</description> <description>Currency</description> <description><c>$#,##0_);($#,##0)</c></description> </item> <item> <description>6</description> <description>Currency</description> <description><c>$#,##0_);[Red]($#,##0)</c></description> </item> <item> <description>7</description> <description>Currency</description> <description><c>$#,##0.00_);($#,##0.00)</c></description> </item> <item> <description>8</description> <description>Currency</description> <description><c>$#,##0.00_);[Red]($#,##0.00)</c></description> </item> <item> <description>9</description> <description>Percentage</description> <description><c>0%</c></description> </item> <item> <description>10</description> <description>Percentage</description> <description><c>0.00%</c></description> </item> <item> <description>11</description> <description>Scientific</description> <description><c>0.00E+00</c></description> </item> <item> <description>12</description> <description>Fraction</description> <description><c># ?/?</c></description> </item> <item> <description>13</description> <description>Fraction</description> <description><c># ??/??</c></description> </item> <item> <description>14</description> <description>Date</description> <description><c>m/d/yyyy</c></description> </item> <item> <description>15</description> <description>Date</description> <description><c>d-mmm-yy</c></description> </item> <item> <description>16</description> <description>Date</description> <description><c>d-mmm</c></description> </item> <item> <description>17</description> <description>Date</description> <description><c>mmm-yy</c></description> </item> <item> <description>18</description> <description>Time</description> <description><c>h:mm AM/PM</c></description> </item> <item> <description>19</description> <description>Time</description> <description><c>h:mm:ss AM/PM</c></description> </item> <item> <description>20</description> <description>Time</description> <description><c>h:mm</c></description> </item> <item> <description>21</description> <description>Time</description> <description><c>h:mm:ss</c></description> </item> <item> <description>22</description> <description>Time</description> <description><c>m/d/yyyy h:mm</c></description> </item> <item> <description>37</description> <description>Accounting</description> <description><c>#,##0_);(#,##0)</c></description> </item> <item> <description>38</description> <description>Accounting</description> <description><c>#,##0_);[Red](#,##0)</c></description> </item> <item> <description>39</description> <description>Accounting</description> <description><c>#,##0.00_);(#,##0.00)</c></description> </item> <item> <description>40</description> <description>Accounting</description> <description><c>#,##0.00_);[Red](#,##0.00)</c></description> </item> <item> <description>41</description> <description>Accounting</description> <description><c>_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)</c></description> </item> <item> <description>42</description> <description>Currency</description> <description><c>_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)</c></description> </item> <item> <description>43</description> <description>Accounting</description> <description><c>_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)</c></description> </item> <item> <description>44</description> <description>Currency</description> <description><c>_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)</c></description> </item> <item> <description>45</description> <description>Time</description> <description><c>mm:ss</c></description> </item> <item> <description>46</description> <description>Time</description> <description><c>[h]:mm:ss</c></description> </item> <item> <description>47</description> <description>Time</description> <description><c>mm:ss.0</c></description> </item> <item> <description>48</description> <description>Scientific</description> <description><c>##0.0E+0</c></description> </item> <item> <description>49</description> <description>Text</description> <description><c>@</c></description> </item> </list

### isLocked() {#isLocked--}

Gets or sets a value indicating whether a cell can be modified or not.

```javascript
isLocked() : boolean;
```


**Remarks**

Locking cells has no effect unless the worksheet is protected.

### setIsLocked(boolean) {#setIsLocked-boolean-}

Gets or sets a value indicating whether a cell can be modified or not.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Locking cells has no effect unless the worksheet is protected.

### getCustom() {#getCustom--}

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.

```javascript
getCustom() : string;
```


**Remarks**

The returned custom string is culture-independent.

### setCustom(string) {#setCustom-string-}

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.

```javascript
setCustom(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The returned custom string is culture-independent.

### getCultureCustom() {#getCultureCustom--}

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```javascript
getCultureCustom() : string;
```


**Remarks**

For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes  "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### setCultureCustom(string) {#setCultureCustom-string-}

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```javascript
setCultureCustom(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes  "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### getInvariantCustom() {#getInvariantCustom--}

Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```javascript
getInvariantCustom() : string;
```


**Remarks**

For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from [CultureCustom](../culturecustom/) is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and  "y" will always be used as the "year" part no matter what other special character is used for the specific locale.

### isFormulaHidden() {#isFormulaHidden--}

Represents if the formula will be hidden when the worksheet is protected.

```javascript
isFormulaHidden() : boolean;
```


### setIsFormulaHidden(boolean) {#setIsFormulaHidden-boolean-}

Represents if the formula will be hidden when the worksheet is protected.

```javascript
setIsFormulaHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShrinkToFit() {#getShrinkToFit--}

Represents if text automatically shrinks to fit in the available column width.

```javascript
getShrinkToFit() : boolean;
```


### setShrinkToFit(boolean) {#setShrinkToFit-boolean-}

Represents if text automatically shrinks to fit in the available column width.

```javascript
setShrinkToFit(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextDirection() {#getTextDirection--}

Represents text reading order.

```javascript
getTextDirection() : TextDirectionType;
```


**Returns**

[TextDirectionType](../textdirectiontype/)

### setTextDirection(TextDirectionType) {#setTextDirection-textdirectiontype-}

Represents text reading order.

```javascript
setTextDirection(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |

### isJustifyDistributed() {#isJustifyDistributed--}

Indicates if the cells justified or distributed alignment should be used on the last line of text.

```javascript
isJustifyDistributed() : boolean;
```


**Remarks**

This is typical for East Asian alignments but not typical in other contexts.

### setIsJustifyDistributed(boolean) {#setIsJustifyDistributed-boolean-}

Indicates if the cells justified or distributed alignment should be used on the last line of text.

```javascript
setIsJustifyDistributed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

This is typical for East Asian alignments but not typical in other contexts.

### getQuotePrefix() {#getQuotePrefix--}

Indicates whether the cell's value starts with single quote mark.

```javascript
getQuotePrefix() : boolean;
```


### setQuotePrefix(boolean) {#setQuotePrefix-boolean-}

Indicates whether the cell's value starts with single quote mark.

```javascript
setQuotePrefix(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isGradient() {#isGradient--}

Indicates whether the cell shading is a gradient pattern.

```javascript
isGradient() : boolean;
```


### setIsGradient(boolean) {#setIsGradient-boolean-}

Indicates whether the cell shading is a gradient pattern.

```javascript
setIsGradient(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isPercent() {#isPercent--}

Indicates whether the number format is a percent format.

```javascript
isPercent() : boolean;
```


### isDateTime() {#isDateTime--}

Indicates whether the number format is a date format.

```javascript
isDateTime() : boolean;
```


### setPatternColor(BackgroundType, Color, Color) {#setPatternColor-backgroundtype-color-color-}

Sets the background color.

```javascript
setPatternColor(pattern: BackgroundType, color1: Color, color2: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | [BackgroundType](../backgroundtype/) | The pattern. |
| color1 | [Color](../color/) | The foreground color. |
| color2 | [Color](../color/) | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |

### copy(Style) {#copy-style-}

Copies data from another style object

```javascript
copy(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | Source Style object |

**Remarks**

This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

### update() {#update--}

Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.

```javascript
update() : void;
```


### isModified(StyleModifyFlag) {#isModified-stylemodifyflag-}

Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.

```javascript
isModified(modifyFlag: StyleModifyFlag) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | [StyleModifyFlag](../stylemodifyflag/) | Style modified flags |

**Returns**

true if the specified properties have been modified

### equals(Object) {#equals-object-}

Determines whether two Style instances are equal.

```javascript
equals(obj: Object) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The Style object to compare with the current Style object. |

**Returns**

true if the specified Object is equal to the current Object; otherwise, false.

### getHashCode() {#getHashCode--}

Serves as a hash function for a Style object.

```javascript
getHashCode() : number;
```


**Returns**

A hash code for the current Object.

**Remarks**

This method is only for internal use.

### setBorder(BorderType, CellBorderType, Color) {#setBorder-bordertype-cellbordertype-color-}

Sets the borders of the style.

```javascript
setBorder(borderType: BorderType, borderStyle: CellBorderType, borderColor: Color) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [BorderType](../bordertype/) | The border(s) to be set, can be combination of [BorderType](../bordertype/). |
| borderStyle | [CellBorderType](../cellbordertype/) | The style of the border. |
| borderColor | [Color](../color/) | The color of the border. |

**Returns**

Whether current border settings have been changed.

### setBorder(BorderType, CellBorderType, CellsColor) {#setBorder-bordertype-cellbordertype-cellscolor-}

Sets the borders of the style.

```javascript
setBorder(borderType: BorderType, borderStyle: CellBorderType, borderColor: CellsColor) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [BorderType](../bordertype/) | The border(s) to be set, can be combination of [BorderType](../bordertype/). |
| borderStyle | [CellBorderType](../cellbordertype/) | The style of the border. |
| borderColor | [CellsColor](../cellscolor/) | The color of the border. |

**Returns**

Whether current border settings have been changed.

### setCustom(string, boolean) {#setCustom-string-boolean-}

Sets the Custom number format string of a cell.

```javascript
setCustom(custom: string, builtinPreference: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| custom | string | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | boolean | If given Custom number format string matches one of the built-in number formats         /// corresponding to current regional settings, whether set the number format as built-in instead of Custom. |

### setTwoColorGradient(Color, Color, GradientStyleType, number) {#setTwoColorGradient-color-color-gradientstyletype-number-}

Sets the specified fill to a two-color gradient.

```javascript
setTwoColorGradient(color1: Color, color2: Color, gradientStyleType: GradientStyleType, variant: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) | One gradient color. |
| color2 | [Color](../color/) | Two gradient color. |
| gradientStyleType | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}

Get the two-color gradient setting.

```javascript
getTwoColorGradientSetting() : TwoColorGradient;
```


**Returns**

[TwoColorGradient](../twocolorgradient/)

### toJson() {#toJson--}

Convert [Style](../style/) to JSON struct data.

```javascript
toJson() : string;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



