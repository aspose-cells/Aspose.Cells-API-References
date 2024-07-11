---
title: FontSettingCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of [FontSetting](./fontsetting/).
type: docs
url: /nodejs-cpp/fontsettingcollection/
---

## FontSettingCollection class

Represents the list of [FontSetting](./fontsetting/).

```javascript
class FontSettingCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [FontSetting](./fontsetting/) by the index. |
| [getTextAlignment()](#getTextAlignment--)| Represents the alignment setting of the text body. |
| [getTextParagraphs()](#getTextParagraphs--)| Gets all paragraphs. |
| [getText()](#getText--)| Gets and sets the text of the shape. |
| [setText(string)](#setText-string-)| Gets and sets the text of the shape. |
| [getHtmlString()](#getHtmlString--)| Gets and sets the html string which contains data and some formats in this shape. |
| [setHtmlString(string)](#setHtmlString-string-)| Gets and sets the html string which contains data and some formats in this shape. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getParagraphEnumerator()](#getParagraphEnumerator--)| Gets the enumerator of the paragraphs. |
| [appendText(string)](#appendText-string-)| Appends the text. |
| [insertText(number, string)](#insertText-number-string-)| Insert index at the position. |
| [replace(number, number, string)](#replace-number-number-string-)| Replace the text. |
| [replace(string, string)](#replace-string-string-)| Replace the text. |
| [deleteText(number, number)](#deleteText-number-number-)| Delete some characters. |
| [format(number, number, Font, StyleFlag)](#format-number-number-font-styleflag-)| Format the text with font setting. |
| [clear()](#clear--)| Clear all setting. |
| [getHashCode()](#getHashCode--)|  |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the [FontSetting](./fontsetting/) by the index.

```javascript
get(index: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[FontSetting](./fontsetting/)

### getTextAlignment() {#getTextAlignment--}

Represents the alignment setting of the text body.

```javascript
getTextAlignment() : ShapeTextAlignment;
```


**Returns**

[ShapeTextAlignment](./shapetextalignment/)

### getTextParagraphs() {#getTextParagraphs--}

Gets all paragraphs.

```javascript
getTextParagraphs() : TextParagraphCollection;
```


**Returns**

[TextParagraphCollection](./textparagraphcollection/)

### getText() {#getText--}

Gets and sets the text of the shape.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Gets and sets the text of the shape.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getHtmlString() {#getHtmlString--}

Gets and sets the html string which contains data and some formats in this shape.

```javascript
getHtmlString() : string;
```


### setHtmlString(string) {#setHtmlString-string-}

Gets and sets the html string which contains data and some formats in this shape.

```javascript
setHtmlString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}

Sets the preset WordArt style.

```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](./presetwordartstyle/) | The preset WordArt style. |

### getParagraphEnumerator() {#getParagraphEnumerator--}

Gets the enumerator of the paragraphs.

```javascript
getParagraphEnumerator() : TextParagraphEnumerator;
```


**Returns**

[TextParagraphEnumerator](./textparagraphenumerator/)

### appendText(string) {#appendText-string-}

Appends the text.

```javascript
appendText(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text. |

### insertText(number, string) {#insertText-number-string-}

Insert index at the position.

```javascript
insertText(index: number, text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The start index. |
| text | string | The text. |

### replace(number, number, string) {#replace-number-number-string-}

Replace the text.

```javascript
replace(index: number, count: number, text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The start index. |
| count | number | The count of characters. |
| text | string | The text. |

### replace(string, string) {#replace-string-string-}

Replace the text.

```javascript
replace(oldValue: string, newValue: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | string | The old text. |
| newValue | string | The new text. |

### deleteText(number, number) {#deleteText-number-number-}

Delete some characters.

```javascript
deleteText(index: number, count: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The start index. |
| count | number | The count of characters. |

### format(number, number, Font, StyleFlag) {#format-number-number-font-styleflag-}

Format the text with font setting.

```javascript
format(startIndex: number, length: number, font: Font, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The start index. |
| length | number | The length. |
| font | [Font](./font/) | The font. |
| flag | [StyleFlag](./styleflag/) | The flags of the font. |

### clear() {#clear--}

Clear all setting.

```javascript
clear() : void;
```


### getHashCode() {#getHashCode--}



```javascript
getHashCode() : number;
```


### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



