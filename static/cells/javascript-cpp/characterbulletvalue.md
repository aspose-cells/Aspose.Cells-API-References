##CharacterBulletValue
Represents the character bullet.
## CharacterBulletValue class
Represents the character bullet.
```javascript
class CharacterBulletValue extends BulletValue;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [character](#character--)| string | Gets and sets character of the bullet. |
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
### character {#character--}
Gets and sets character of the bullet.
```javascript
character : string;
```
### getType() {#getType--}
Gets the type of the bullet.
```javascript
getType() : BulletType;
```
**Returns**
[BulletType](../bullettype/)
