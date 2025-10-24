##AutoNumberedBulletValue
Represents automatic numbered bullet.
## AutoNumberedBulletValue class
Represents automatic numbered bullet.
```javascript
class AutoNumberedBulletValue extends BulletValue;
```
## Constructors
| Constructor | Description |
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
| [getStartAt()](#getStartAt--)| <b>@deprecated.</b> Please use the 'startAt' property instead. Gets and sets the starting number of the bullet. |
| [setStartAt(number)](#setStartAt-number-)| <b>@deprecated.</b> Please use the 'startAt' property instead. Gets and sets the starting number of the bullet. |
| [getAutonumberScheme()](#getAutonumberScheme--)| <b>@deprecated.</b> Please use the 'autonumberScheme' property instead. Represents the scheme of automatic number. |
| [setAutonumberScheme(TextAutonumberScheme)](#setAutonumberScheme-textautonumberscheme-)| <b>@deprecated.</b> Please use the 'autonumberScheme' property instead. Represents the scheme of automatic number. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getStartAt() {#getStartAt--}
```javascript
getStartAt() : number;
```
### setStartAt(number) {#setStartAt-number-}
```javascript
setStartAt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAutonumberScheme() {#getAutonumberScheme--}
```javascript
getAutonumberScheme() : TextAutonumberScheme;
```
**Returns**
[TextAutonumberScheme](../textautonumberscheme/)
### setAutonumberScheme(TextAutonumberScheme) {#setAutonumberScheme-textautonumberscheme-}
```javascript
setAutonumberScheme(value: TextAutonumberScheme) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAutonumberScheme](../textautonumberscheme/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getType() {#getType--}
Gets the type of the bullet.
```javascript
getType() : BulletType;
```
**Returns**
[BulletType](../bullettype/)
