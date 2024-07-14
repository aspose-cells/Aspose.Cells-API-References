---
title: Font
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the font object used in a spreadsheet.
type: docs
url: /nodejs-cpp/font/
---

## Font class

Encapsulates the font object used in a spreadsheet.

```javascript
class Font;
```


## Methods

| Method | Description |
| --- | --- |
| [getCharset()](#getCharset--)| Represent the character set. |
| [setCharset(number)](#setCharset-number-)| Represent the character set. |
| [isItalic()](#isItalic--)| Gets or sets a value indicating whether the font is italic. |
| [setIsItalic(boolean)](#setIsItalic-boolean-)| Gets or sets a value indicating whether the font is italic. |
| [isBold()](#isBold--)| Gets or sets a value indicating whether the font is bold. |
| [setIsBold(boolean)](#setIsBold-boolean-)| Gets or sets a value indicating whether the font is bold. |
| [getCapsType()](#getCapsType--)| Gets and sets the text caps type. |
| [setCapsType(TextCapsType)](#setCapsType-textcapstype-)| Gets and sets the text caps type. |
| [getStrikeType()](#getStrikeType--)| Gets the strike type of the text. |
| [setStrikeType(TextStrikeType)](#setStrikeType-textstriketype-)| Gets the strike type of the text. |
| [isStrikeout()](#isStrikeout--)| Gets or sets a value indicating whether the font is single strikeout. |
| [setIsStrikeout(boolean)](#setIsStrikeout-boolean-)| Gets or sets a value indicating whether the font is single strikeout. |
| [getScriptOffset()](#getScriptOffset--)| Gets and sets the script offset,in unit of percentage |
| [setScriptOffset(number)](#setScriptOffset-number-)| Gets and sets the script offset,in unit of percentage |
| [isSuperscript()](#isSuperscript--)| Gets or sets a value indicating whether the font is super script. |
| [setIsSuperscript(boolean)](#setIsSuperscript-boolean-)| Gets or sets a value indicating whether the font is super script. |
| [isSubscript()](#isSubscript--)| Gets or sets a value indicating whether the font is subscript. |
| [setIsSubscript(boolean)](#setIsSubscript-boolean-)| Gets or sets a value indicating whether the font is subscript. |
| [getUnderline()](#getUnderline--)| Gets or sets the font underline type. |
| [setUnderline(FontUnderlineType)](#setUnderline-fontunderlinetype-)| Gets or sets the font underline type. |
| [getDoubleSize()](#getDoubleSize--)| Gets and sets the double size of the font. |
| [setDoubleSize(number)](#setDoubleSize-number-)| Gets and sets the double size of the font. |
| [getSize()](#getSize--)| Gets or sets the size of the font. |
| [setSize(number)](#setSize-number-)| Gets or sets the size of the font. |
| [getThemeColor()](#getThemeColor--)| Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets and sets the theme color. |
| [getColor()](#getColor--)| Gets or sets the [System.Drawing.Color](/nodejs-cpp/system.drawing.color/) of the font. |
| [setColor(Color)](#setColor-color-)| Gets or sets the [System.Drawing.Color](/nodejs-cpp/system.drawing.color/) of the font. |
| [getArgbColor()](#getArgbColor--)| Gets and sets the color with a 32-bit ARGB value. |
| [setArgbColor(number)](#setArgbColor-number-)| Gets and sets the color with a 32-bit ARGB value. |
| [isNormalizeHeights()](#isNormalizeHeights--)| Indicates whether the normalization of height that is to be applied to the text run. |
| [setIsNormalizeHeights(boolean)](#setIsNormalizeHeights-boolean-)| Indicates whether the normalization of height that is to be applied to the text run. |
| [getSchemeType()](#getSchemeType--)| Gets and sets the scheme type of the font. |
| [setSchemeType(FontSchemeType)](#setSchemeType-fontschemetype-)| Gets and sets the scheme type of the font. |
| [equals(Font)](#equals-font-)| Checks if two fonts are equals. |
| [toString()](#toString--)| Returns a string represents the current Cell object. |
| [getName()](#getName--)| Gets  or sets the name of the [Font](/nodejs-cpp/font/). |
| [setName(string)](#setName-string-)| Gets  or sets the name of the [Font](/nodejs-cpp/font/). |


### getCharset() {#getCharset--}

Represent the character set.

```javascript
getCharset() : number;
```


### setCharset(number) {#setCharset-number-}

Represent the character set.

```javascript
setCharset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isItalic() {#isItalic--}

Gets or sets a value indicating whether the font is italic.

```javascript
isItalic() : boolean;
```


### setIsItalic(boolean) {#setIsItalic-boolean-}

Gets or sets a value indicating whether the font is italic.

```javascript
setIsItalic(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isBold() {#isBold--}

Gets or sets a value indicating whether the font is bold.

```javascript
isBold() : boolean;
```


### setIsBold(boolean) {#setIsBold-boolean-}

Gets or sets a value indicating whether the font is bold.

```javascript
setIsBold(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCapsType() {#getCapsType--}

Gets and sets the text caps type.

```javascript
getCapsType() : TextCapsType;
```


**Returns**

[TextCapsType](/nodejs-cpp/textcapstype/)

### setCapsType(TextCapsType) {#setCapsType-textcapstype-}

Gets and sets the text caps type.

```javascript
setCapsType(value: TextCapsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCapsType](/nodejs-cpp/textcapstype/) | The value to set. |

### getStrikeType() {#getStrikeType--}

Gets the strike type of the text.

```javascript
getStrikeType() : TextStrikeType;
```


**Returns**

[TextStrikeType](/nodejs-cpp/textstriketype/)

### setStrikeType(TextStrikeType) {#setStrikeType-textstriketype-}

Gets the strike type of the text.

```javascript
setStrikeType(value: TextStrikeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextStrikeType](/nodejs-cpp/textstriketype/) | The value to set. |

### isStrikeout() {#isStrikeout--}

Gets or sets a value indicating whether the font is single strikeout.

```javascript
isStrikeout() : boolean;
```


### setIsStrikeout(boolean) {#setIsStrikeout-boolean-}

Gets or sets a value indicating whether the font is single strikeout.

```javascript
setIsStrikeout(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getScriptOffset() {#getScriptOffset--}

Gets and sets the script offset,in unit of percentage

```javascript
getScriptOffset() : number;
```


### setScriptOffset(number) {#setScriptOffset-number-}

Gets and sets the script offset,in unit of percentage

```javascript
setScriptOffset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isSuperscript() {#isSuperscript--}

Gets or sets a value indicating whether the font is super script.

```javascript
isSuperscript() : boolean;
```


### setIsSuperscript(boolean) {#setIsSuperscript-boolean-}

Gets or sets a value indicating whether the font is super script.

```javascript
setIsSuperscript(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isSubscript() {#isSubscript--}

Gets or sets a value indicating whether the font is subscript.

```javascript
isSubscript() : boolean;
```


### setIsSubscript(boolean) {#setIsSubscript-boolean-}

Gets or sets a value indicating whether the font is subscript.

```javascript
setIsSubscript(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUnderline() {#getUnderline--}

Gets or sets the font underline type.

```javascript
getUnderline() : FontUnderlineType;
```


**Returns**

[FontUnderlineType](/nodejs-cpp/fontunderlinetype/)

### setUnderline(FontUnderlineType) {#setUnderline-fontunderlinetype-}

Gets or sets the font underline type.

```javascript
setUnderline(value: FontUnderlineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontUnderlineType](/nodejs-cpp/fontunderlinetype/) | The value to set. |

### getDoubleSize() {#getDoubleSize--}

Gets and sets the double size of the font.

```javascript
getDoubleSize() : number;
```


### setDoubleSize(number) {#setDoubleSize-number-}

Gets and sets the double size of the font.

```javascript
setDoubleSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSize() {#getSize--}

Gets or sets the size of the font.

```javascript
getSize() : number;
```


### setSize(number) {#setSize-number-}

Gets or sets the size of the font.

```javascript
setSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getThemeColor() {#getThemeColor--}

Gets and sets the theme color.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](/nodejs-cpp/themecolor/)

**Remarks**

If the font color is not a theme color, NULL will be returned.

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets and sets the theme color.

```javascript
setThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](/nodejs-cpp/themecolor/) | The value to set. |

**Remarks**

If the font color is not a theme color, NULL will be returned.

### getColor() {#getColor--}

Gets or sets the [System.Drawing.Color](/nodejs-cpp/system.drawing.color/) of the font.

```javascript
getColor() : Color;
```


**Returns**

[Color](/nodejs-cpp/color/)

### setColor(Color) {#setColor-color-}

Gets or sets the [System.Drawing.Color](/nodejs-cpp/system.drawing.color/) of the font.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](/nodejs-cpp/color/) | The value to set. |

### getArgbColor() {#getArgbColor--}

Gets and sets the color with a 32-bit ARGB value.

```javascript
getArgbColor() : number;
```


### setArgbColor(number) {#setArgbColor-number-}

Gets and sets the color with a 32-bit ARGB value.

```javascript
setArgbColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNormalizeHeights() {#isNormalizeHeights--}

Indicates whether the normalization of height that is to be applied to the text run.

```javascript
isNormalizeHeights() : boolean;
```


### setIsNormalizeHeights(boolean) {#setIsNormalizeHeights-boolean-}

Indicates whether the normalization of height that is to be applied to the text run.

```javascript
setIsNormalizeHeights(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSchemeType() {#getSchemeType--}

Gets and sets the scheme type of the font.

```javascript
getSchemeType() : FontSchemeType;
```


**Returns**

[FontSchemeType](/nodejs-cpp/fontschemetype/)

### setSchemeType(FontSchemeType) {#setSchemeType-fontschemetype-}

Gets and sets the scheme type of the font.

```javascript
setSchemeType(value: FontSchemeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontSchemeType](/nodejs-cpp/fontschemetype/) | The value to set. |

### equals(Font) {#equals-font-}

Checks if two fonts are equals.

```javascript
equals(font: Font) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| font | [Font](/nodejs-cpp/font/) | Compared font object. |

**Returns**

True if equal to the compared font object.

### toString() {#toString--}

Returns a string represents the current Cell object.

```javascript
toString() : string;
```


### getName() {#getName--}

Gets  or sets the name of the [Font](/nodejs-cpp/font/).

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets  or sets the name of the [Font](/nodejs-cpp/font/).

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |


