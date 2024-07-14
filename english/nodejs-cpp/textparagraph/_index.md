---
title: TextParagraph
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the text paragraph setting.
type: docs
url: /nodejs-cpp/textparagraph/
---

## TextParagraph class

Represents the text paragraph setting.

```javascript
class TextParagraph extends FontSetting;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(FontSetting)](#constructor-fontsetting-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getBullet()](#getBullet--)| Gets the bullet. |
| [getType()](#getType--)| Gets the type of text node. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--)| Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [setLineSpaceSizeType(LineSpaceSizeType)](#setLineSpaceSizeType-linespacesizetype-)| Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getLineSpace()](#getLineSpace--)| Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [setLineSpace(number)](#setLineSpace-number-)| Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--)| Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [setSpaceAfterSizeType(LineSpaceSizeType)](#setSpaceAfterSizeType-linespacesizetype-)| Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceAfter()](#getSpaceAfter--)| Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [setSpaceAfter(number)](#setSpaceAfter-number-)| Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--)| Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [setSpaceBeforeSizeType(LineSpaceSizeType)](#setSpaceBeforeSizeType-linespacesizetype-)| Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getSpaceBefore()](#getSpaceBefore--)| Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [setSpaceBefore(number)](#setSpaceBefore-number-)| Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getStops()](#getStops--)| Gets tab stop list. |
| [isLatinLineBreak()](#isLatinLineBreak--)| Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [setIsLatinLineBreak(boolean)](#setIsLatinLineBreak-boolean-)| Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--)| Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [setIsEastAsianLineBreak(boolean)](#setIsEastAsianLineBreak-boolean-)| Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isHangingPunctuation()](#isHangingPunctuation--)| Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [setIsHangingPunctuation(boolean)](#setIsHangingPunctuation-boolean-)| Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [getRightMargin()](#getRightMargin--)| Specifies the right margin of the paragraph. |
| [setRightMargin(number)](#setRightMargin-number-)| Specifies the right margin of the paragraph. |
| [getLeftMargin()](#getLeftMargin--)| Specifies the left margin of the paragraph. |
| [setLeftMargin(number)](#setLeftMargin-number-)| Specifies the left margin of the paragraph. |
| [getFirstLineIndent()](#getFirstLineIndent--)| Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [setFirstLineIndent(number)](#setFirstLineIndent-number-)| Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [getFontAlignType()](#getFontAlignType--)| Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [setFontAlignType(TextFontAlignType)](#setFontAlignType-textfontaligntype-)| Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [getAlignmentType()](#getAlignmentType--)| Gets and sets the text horizontal alignment type of the paragraph. |
| [setAlignmentType(TextAlignmentType)](#setAlignmentType-textalignmenttype-)| Gets and sets the text horizontal alignment type of the paragraph. |
| [getDefaultTabSize()](#getDefaultTabSize--)| Gets and sets the default size for a tab character within this paragraph. |
| [setDefaultTabSize(number)](#setDefaultTabSize-number-)| Gets and sets the default size for a tab character within this paragraph. |
| [getChildren()](#getChildren--)| Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [getStartIndex()](#getStartIndex--)| Gets the start index of the characters. |
| [getLength()](#getLength--)| Gets the length of the characters. |
| [getFont()](#getFont--)| Returns the font of this object. |
| [getTextOptions()](#getTextOptions--)| Returns the text options. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |


### constructor(FontSetting) {#constructor-fontsetting-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: FontSetting);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSetting | The parent object. |

### getBullet() {#getBullet--}

Gets the bullet.

```javascript
getBullet() : Bullet;
```


**Returns**

[Bullet](/nodejs-cpp/bullet/)

### getType() {#getType--}

Gets the type of text node.

```javascript
getType() : TextNodeType;
```


**Returns**

[TextNodeType](/nodejs-cpp/textnodetype/)

### getLineSpaceSizeType() {#getLineSpaceSizeType--}

Gets and sets the amount of vertical white space that will be used within a paragraph.

```javascript
getLineSpaceSizeType() : LineSpaceSizeType;
```


**Returns**

[LineSpaceSizeType](/nodejs-cpp/linespacesizetype/)

### setLineSpaceSizeType(LineSpaceSizeType) {#setLineSpaceSizeType-linespacesizetype-}

Gets and sets the amount of vertical white space that will be used within a paragraph.

```javascript
setLineSpaceSizeType(value: LineSpaceSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](/nodejs-cpp/linespacesizetype/) | The value to set. |

### getLineSpace() {#getLineSpace--}

Gets and sets the amount of vertical white space that will be used within a paragraph.

```javascript
getLineSpace() : number;
```


### setLineSpace(number) {#setLineSpace-number-}

Gets and sets the amount of vertical white space that will be used within a paragraph.

```javascript
setLineSpace(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}

Gets and sets the amount of vertical white space that will be present after a paragraph.

```javascript
getSpaceAfterSizeType() : LineSpaceSizeType;
```


**Returns**

[LineSpaceSizeType](/nodejs-cpp/linespacesizetype/)

### setSpaceAfterSizeType(LineSpaceSizeType) {#setSpaceAfterSizeType-linespacesizetype-}

Gets and sets the amount of vertical white space that will be present after a paragraph.

```javascript
setSpaceAfterSizeType(value: LineSpaceSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](/nodejs-cpp/linespacesizetype/) | The value to set. |

### getSpaceAfter() {#getSpaceAfter--}

Gets and sets the amount of vertical white space that will be present after a paragraph.

```javascript
getSpaceAfter() : number;
```


### setSpaceAfter(number) {#setSpaceAfter-number-}

Gets and sets the amount of vertical white space that will be present after a paragraph.

```javascript
setSpaceAfter(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}

Gets and sets the amount of vertical white space that will be present before a paragraph.

```javascript
getSpaceBeforeSizeType() : LineSpaceSizeType;
```


**Returns**

[LineSpaceSizeType](/nodejs-cpp/linespacesizetype/)

### setSpaceBeforeSizeType(LineSpaceSizeType) {#setSpaceBeforeSizeType-linespacesizetype-}

Gets and sets the amount of vertical white space that will be present before a paragraph.

```javascript
setSpaceBeforeSizeType(value: LineSpaceSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](/nodejs-cpp/linespacesizetype/) | The value to set. |

### getSpaceBefore() {#getSpaceBefore--}

Gets and sets the amount of vertical white space that will be present before a paragraph.

```javascript
getSpaceBefore() : number;
```


### setSpaceBefore(number) {#setSpaceBefore-number-}

Gets and sets the amount of vertical white space that will be present before a paragraph.

```javascript
setSpaceBefore(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStops() {#getStops--}

Gets tab stop list.

```javascript
getStops() : TextTabStopCollection;
```


**Returns**

[TextTabStopCollection](/nodejs-cpp/texttabstopcollection/)

### isLatinLineBreak() {#isLatinLineBreak--}

Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.

```javascript
isLatinLineBreak() : boolean;
```


### setIsLatinLineBreak(boolean) {#setIsLatinLineBreak-boolean-}

Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.

```javascript
setIsLatinLineBreak(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isEastAsianLineBreak() {#isEastAsianLineBreak--}

Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.

```javascript
isEastAsianLineBreak() : boolean;
```


### setIsEastAsianLineBreak(boolean) {#setIsEastAsianLineBreak-boolean-}

Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.

```javascript
setIsEastAsianLineBreak(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHangingPunctuation() {#isHangingPunctuation--}

Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.

```javascript
isHangingPunctuation() : boolean;
```


### setIsHangingPunctuation(boolean) {#setIsHangingPunctuation-boolean-}

Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.

```javascript
setIsHangingPunctuation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRightMargin() {#getRightMargin--}

Specifies the right margin of the paragraph.

```javascript
getRightMargin() : number;
```


### setRightMargin(number) {#setRightMargin-number-}

Specifies the right margin of the paragraph.

```javascript
setRightMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftMargin() {#getLeftMargin--}

Specifies the left margin of the paragraph.

```javascript
getLeftMargin() : number;
```


### setLeftMargin(number) {#setLeftMargin-number-}

Specifies the left margin of the paragraph.

```javascript
setLeftMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFirstLineIndent() {#getFirstLineIndent--}

Specifies the indent size that will be applied to the first line of text in the paragraph.

```javascript
getFirstLineIndent() : number;
```


### setFirstLineIndent(number) {#setFirstLineIndent-number-}

Specifies the indent size that will be applied to the first line of text in the paragraph.

```javascript
setFirstLineIndent(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFontAlignType() {#getFontAlignType--}

Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines.

```javascript
getFontAlignType() : TextFontAlignType;
```


**Returns**

[TextFontAlignType](/nodejs-cpp/textfontaligntype/)

### setFontAlignType(TextFontAlignType) {#setFontAlignType-textfontaligntype-}

Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines.

```javascript
setFontAlignType(value: TextFontAlignType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextFontAlignType](/nodejs-cpp/textfontaligntype/) | The value to set. |

### getAlignmentType() {#getAlignmentType--}

Gets and sets the text horizontal alignment type of the paragraph.

```javascript
getAlignmentType() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](/nodejs-cpp/textalignmenttype/)

### setAlignmentType(TextAlignmentType) {#setAlignmentType-textalignmenttype-}

Gets and sets the text horizontal alignment type of the paragraph.

```javascript
setAlignmentType(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](/nodejs-cpp/textalignmenttype/) | The value to set. |

### getDefaultTabSize() {#getDefaultTabSize--}

Gets and sets the default size for a tab character within this paragraph.

```javascript
getDefaultTabSize() : number;
```


### setDefaultTabSize(number) {#setDefaultTabSize-number-}

Gets and sets the default size for a tab character within this paragraph.

```javascript
setDefaultTabSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getChildren() {#getChildren--}

Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.

```javascript
getChildren() : FontSetting[];
```


**Returns**

[FontSetting](/nodejs-cpp/fontsetting/)[]

### getStartIndex() {#getStartIndex--}

Gets the start index of the characters.

```javascript
getStartIndex() : number;
```


### getLength() {#getLength--}

Gets the length of the characters.

```javascript
getLength() : number;
```


### getFont() {#getFont--}

Returns the font of this object.

```javascript
getFont() : Font;
```


**Returns**

[Font](/nodejs-cpp/font/)

### getTextOptions() {#getTextOptions--}

Returns the text options.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](/nodejs-cpp/textoptions/)

### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}

Sets the preset WordArt style.

```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](/nodejs-cpp/presetwordartstyle/) | The preset WordArt style. |

**Remarks**

Only for the text of shape/chart.


