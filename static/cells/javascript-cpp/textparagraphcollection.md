##TextParagraphCollection
Represents all text paragraph.
## TextParagraphCollection class
Represents all text paragraph.
```javascript
class TextParagraphCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of text paragraphs. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [TextParagraph](../textparagraph/) object at specific index. |
| [getEnumerator()](#getEnumerator--)| Gets the enumerator of the paragraphs. |
### count {#count--}
Readonly. Gets the count of text paragraphs.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets the [TextParagraph](../textparagraph/) object at specific index.
```javascript
get(index: number) : TextParagraph;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[TextParagraph](../textparagraph/)
### getEnumerator() {#getEnumerator--}
Gets the enumerator of the paragraphs.
```javascript
getEnumerator() : TextParagraphEnumerator;
```
**Returns**
[TextParagraphEnumerator](../textparagraphenumerator/)
