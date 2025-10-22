##ProtectedRange
A specified range to be allowed to edit when the sheet protection is ON.
## ProtectedRange class
A specified range to be allowed to edit when the sheet protection is ON.
```javascript
class ProtectedRange;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the [CellArea](../cellarea/) object represents the cell area to be protected. |
| [isProtectedWithPassword](#isProtectedWithPassword--)| boolean | Readonly. Indicates whether the worksheets is protected with password. |
| [password](#password--)| string | Represents the password to protect the range. |
| [securityDescriptor](#securityDescriptor--)| string | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
## Methods
| Method | Description |
| --- | --- |
| [getAreas()](#getAreas--)| Gets all referred areas. |
| [addArea(number, number, number, number)](#addArea-number-number-number-number-)| Adds a referred area to this |
### name {#name--}
Gets the Range title. This is used as a descriptor, not as a named range definition.
```javascript
name : string;
```
### cellArea {#cellArea--}
Readonly. Gets the [CellArea](../cellarea/) object represents the cell area to be protected.
```javascript
cellArea : CellArea;
```
### isProtectedWithPassword {#isProtectedWithPassword--}
Readonly. Indicates whether the worksheets is protected with password.
```javascript
isProtectedWithPassword : boolean;
```
### password {#password--}
Represents the password to protect the range.
```javascript
password : string;
```
### securityDescriptor {#securityDescriptor--}
The security descriptor defines user accounts who may edit this range without providing a password to access the range.
```javascript
securityDescriptor : string;
```
### getAreas() {#getAreas--}
Gets all referred areas.
```javascript
getAreas() : CellArea[];
```
**Returns**
Returns all referred areas.
### addArea(number, number, number, number) {#addArea-number-number-number-number-}
Adds a referred area to this
```javascript
addArea(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row. |
| startColumn | number | The start column. |
| endRow | number | The end row. |
| endColumn | number | The end column. |
