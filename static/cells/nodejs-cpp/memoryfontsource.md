##MemoryFontSource
Represents the single TrueType font file stored in memory.
## MemoryFontSource class
Represents the single TrueType font file stored in memory.
```javascript
class MemoryFontSource extends FontSourceBase;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(Uint8Array)](#constructor-uint8array-)| Ctor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [fontData](#fontData--)| Uint8Array | Readonly. Binary font data. |
## Methods
| Method | Description |
| --- | --- |
| [getFontData()](#getFontData--)| <b>@deprecated.</b> Please use the 'fontData' property instead. Binary font data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getType()](#getType--)| Returns the type of the font source. |
### constructor(FontSourceBase) {#constructor-fontsourcebase-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: FontSourceBase);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSourceBase | The parent object. |
### constructor(Uint8Array) {#constructor-uint8array-}
Ctor.
```javascript
constructor(fontData: Uint8Array);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontData | number[] | Binary font data. |
### fontData {#fontData--}
Readonly. Binary font data.
```javascript
fontData : Uint8Array;
```
### getFontData() {#getFontData--}
```javascript
getFontData() : Uint8Array;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getType() {#getType--}
Returns the type of the font source.
```javascript
getType() : FontSourceType;
```
**Returns**
[FontSourceType](../fontsourcetype/)
