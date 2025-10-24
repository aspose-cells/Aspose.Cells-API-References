##FileFontSource
Represents the single TrueType font file stored in the file system.
## FileFontSource class
Represents the single TrueType font file stored in the file system.
```javascript
class FileFontSource extends FontSourceBase;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(string)](#constructor-string-)| Ctor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [filePath](#filePath--)| string | Readonly. Path to font file. |
## Methods
| Method | Description |
| --- | --- |
| [getFilePath()](#getFilePath--)| <b>@deprecated.</b> Please use the 'filePath' property instead. Path to font file. |
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
### constructor(string) {#constructor-string-}
Ctor.
```javascript
constructor(filePath: string);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | string | path to font file |
### filePath {#filePath--}
Readonly. Path to font file.
```javascript
filePath : string;
```
### getFilePath() {#getFilePath--}
```javascript
getFilePath() : string;
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
