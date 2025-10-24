##RevisionInsertSheet
Represents a revision record of a sheet that was inserted.
## RevisionInsertSheet class
Represents a revision record of a sheet that was inserted.
```javascript
class RevisionInsertSheet extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the action type of the revision. |
| [name](#name--)| string | Readonly. Gets the name of the worksheet. |
| [sheetPosition](#sheetPosition--)| number | Readonly. Gets the zero based position of the new sheet in the sheet tab bar. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of revision. |
### constructor(Revision) {#constructor-revision-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Revision);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Revision | The parent object. |
### actionType {#actionType--}
Readonly. Gets the action type of the revision.
```javascript
actionType : RevisionActionType;
```
### name {#name--}
Readonly. Gets the name of the worksheet.
```javascript
name : string;
```
### sheetPosition {#sheetPosition--}
Readonly. Gets the zero based position of the new sheet in the sheet tab bar.
```javascript
sheetPosition : number;
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
### getType() {#getType--}
Gets the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
