##Bullet
Represents the bullet points should be applied to a paragraph.
## Bullet class
Represents the bullet points should be applied to a paragraph.
```javascript
class Bullet;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [bulletValue](#bulletValue--)| BulletValue | Readonly. Gets the value of bullet. |
| [type](#type--)| BulletType | Gets and sets the type of bullet. |
| [fontName](#fontName--)| string | Get and sets the name of the font. |
## Methods
| Method | Description |
| --- | --- |
| [getBulletValue()](#getBulletValue--)| <b>@deprecated.</b> Please use the 'bulletValue' property instead. Gets the value of bullet. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the type of bullet. |
| [setType(BulletType)](#setType-bullettype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the type of bullet. |
| [getFontName()](#getFontName--)| <b>@deprecated.</b> Please use the 'fontName' property instead. Get and sets the name of the font. |
| [setFontName(string)](#setFontName-string-)| <b>@deprecated.</b> Please use the 'fontName' property instead. Get and sets the name of the font. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### bulletValue {#bulletValue--}
Readonly. Gets the value of bullet.
```javascript
bulletValue : BulletValue;
```
### type {#type--}
Gets and sets the type of bullet.
```javascript
type : BulletType;
```
### fontName {#fontName--}
Get and sets the name of the font.
```javascript
fontName : string;
```
### getBulletValue() {#getBulletValue--}
```javascript
getBulletValue() : BulletValue;
```
**Returns**
[BulletValue](../bulletvalue/)
### getType() {#getType--}
```javascript
getType() : BulletType;
```
**Returns**
[BulletType](../bullettype/)
### setType(BulletType) {#setType-bullettype-}
```javascript
setType(value: BulletType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BulletType](../bullettype/) | The value to set. |
### getFontName() {#getFontName--}
```javascript
getFontName() : string;
```
### setFontName(string) {#setFontName-string-}
```javascript
setFontName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
