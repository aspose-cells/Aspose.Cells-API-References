##RevisionRenameSheet
Represents a revision of renaming sheet.
## RevisionRenameSheet class
Represents a revision of renaming sheet.
```javascript
class RevisionRenameSheet extends Revision;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [oldName](#oldName--)| string | Readonly. Gets the old name of the worksheet. |
| [newName](#newName--)| string | Readonly. Gets the new name of the worksheet. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getOldName()](#getOldName--)| <b>@deprecated.</b> Please use the 'oldName' property instead. Gets the old name of the worksheet. |
| [getNewName()](#getNewName--)| <b>@deprecated.</b> Please use the 'newName' property instead. Gets the new name of the worksheet. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the worksheet. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the number of this revision. |
| [getType()](#getType--)| Represents the type of the revision. |
### constructor(Revision) {#constructor-revision-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Revision);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Revision | The parent object. |
### oldName {#oldName--}
Readonly. Gets the old name of the worksheet.
```javascript
oldName : string;
```
### newName {#newName--}
Readonly. Gets the new name of the worksheet.
```javascript
newName : string;
```
### worksheet {#worksheet--}
Readonly. Gets the worksheet.
```javascript
worksheet : Worksheet;
```
### id {#id--}
Readonly. Gets the number of this revision.
```javascript
id : number;
```
**Remarks**
Zero means this revision does not contains id.
### getOldName() {#getOldName--}
```javascript
getOldName() : string;
```
### getNewName() {#getNewName--}
```javascript
getNewName() : string;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getWorksheet() {#getWorksheet--}
```javascript
getWorksheet() : Worksheet;
```
**Returns**
[Worksheet](../worksheet/)
### getId() {#getId--}
```javascript
getId() : number;
```
**Remarks**
Zero means this revision does not contains id.
### getType() {#getType--}
Represents the type of the revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
