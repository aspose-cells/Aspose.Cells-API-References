##AutoNumberedBulletValue
Represents automatic numbered bullet.
## AutoNumberedBulletValue class
Represents automatic numbered bullet.
```javascript
class AutoNumberedBulletValue extends BulletValue;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [startAt](#startAt--)| number | Gets and sets the starting number of the bullet. |
| [autonumberScheme](#autonumberScheme--)| TextAutonumberScheme | Represents the scheme of automatic number. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the bullet. |
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
### startAt {#startAt--}
Gets and sets the starting number of the bullet.
```javascript
startAt : number;
```
### autonumberScheme {#autonumberScheme--}
Represents the scheme of automatic number.
```javascript
autonumberScheme : TextAutonumberScheme;
```
### getType() {#getType--}
Gets the type of the bullet.
```javascript
getType() : BulletType;
```
**Returns**
[BulletType](../bullettype/)
