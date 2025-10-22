##CustomPiovtFieldGroupItem
Represents an item of custom grouped field.
## CustomPiovtFieldGroupItem class
Represents an item of custom grouped field.
```javascript
class CustomPiovtFieldGroupItem;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(string, number[])](#constructor-string-numberarray-)| The constructor of custom group item of pivot field. |
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(string, number[]) {#constructor-string-numberarray-}
The constructor of custom group item of pivot field.
```javascript
constructor(name: string, itemIndexes: number[]);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of group item |
| itemIndexes | number[] | All indexes to the items of base pivot field. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
