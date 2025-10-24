##NoneBulletValue
Represents no bullet.
## NoneBulletValue class
Represents no bullet.
```javascript
class NoneBulletValue extends BulletValue;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
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
