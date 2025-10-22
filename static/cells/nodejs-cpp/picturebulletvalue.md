##PictureBulletValue
Represents the value of the image bullet.
## PictureBulletValue class
Represents the value of the image bullet.
```javascript
class PictureBulletValue extends BulletValue;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [imageData](#imageData--)| Uint8Array | Gets and sets image data of the bullet. |
## Methods
| Method | Description |
| --- | --- |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets image data of the bullet. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets image data of the bullet. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getType()](#getType--)| Gets the type of the bullet's value. |
### constructor(BulletValue) {#constructor-bulletvalue-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: BulletValue);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | BulletValue | The parent object. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### imageData {#imageData--}
Gets and sets image data of the bullet.
```javascript
imageData : Uint8Array;
```
### getImageData() {#getImageData--}
```javascript
getImageData() : Uint8Array;
```
### setImageData(Uint8Array) {#setImageData-uint8array-}
```javascript
setImageData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getType() {#getType--}
Gets the type of the bullet's value.
```javascript
getType() : BulletType;
```
**Returns**
[BulletType](../bullettype/)
