##FontSettingCollection
Represents the list of FontSetting..fontsetting.
## FontSettingCollection class
Represents the list of [FontSetting](../fontsetting/).
```javascript
class FontSettingCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [textAlignment](#textAlignment--)| ShapeTextAlignment | Readonly. Represents the alignment setting of the text body. |
| [textParagraphs](#textParagraphs--)| TextParagraphCollection | Readonly. Gets all paragraphs. |
| [text](#text--)| string | Gets and sets the text of the shape. |
| [htmlString](#htmlString--)| string | Gets and sets the html string which contains data and some formats in this shape. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [FontSetting](../fontsetting/) by the index. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getParagraphEnumerator()](#getParagraphEnumerator--)| Gets the enumerator of the paragraphs. |
| [appendText(string)](#appendText-string-)| Appends the text. |
| [insertText(number, string)](#insertText-number-string-)| Insert index at the position. |
| [replace(number, number, string)](#replace-number-number-string-)| Replace the text. |
| [replace(string, string)](#replace-string-string-)| Replace the text. |
| [deleteText(number, number)](#deleteText-number-number-)| Delete some characters. |
| [format(number, number, Font, StyleFlag)](#format-number-number-font-styleflag-)| Format the text with font setting. |
| [clear()](#clear--)| Clear all setting. |
| [equals(VObject)](#equals-vobject-)|  |
| [getHashCode()](#getHashCode--)|  |
### textAlignment {#textAlignment--}
Readonly. Represents the alignment setting of the text body.
```javascript
textAlignment : ShapeTextAlignment;
```
### textParagraphs {#textParagraphs--}
Readonly. Gets all paragraphs.
```javascript
textParagraphs : TextParagraphCollection;
```
### text {#text--}
Gets and sets the text of the shape.
```javascript
text : string;
```
### htmlString {#htmlString--}
Gets and sets the html string which contains data and some formats in this shape.
```javascript
htmlString : string;
```
### get(number) {#get-number-}
Gets the [FontSetting](../fontsetting/) by the index.
```javascript
get(index: number) : FontSetting;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[FontSetting](../fontsetting/)
### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}
Sets the preset WordArt style.
```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](../presetwordartstyle/) | The preset WordArt style. |
### getParagraphEnumerator() {#getParagraphEnumerator--}
Gets the enumerator of the paragraphs.
```javascript
getParagraphEnumerator() : TextParagraphEnumerator;
```
**Returns**
[TextParagraphEnumerator](../textparagraphenumerator/)
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
| font | [Font](../font/) | The font. |
| flag | [StyleFlag](../styleflag/) | The flags of the font. |
### clear() {#clear--}
Clear all setting.
```javascript
clear() : void;
```
### equals(VObject) {#equals-vobject-}
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject |  |
### getHashCode() {#getHashCode--}
```javascript
getHashCode() : number;
```
