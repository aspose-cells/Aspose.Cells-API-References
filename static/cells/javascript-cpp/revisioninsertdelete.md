##RevisionInsertDelete
Represents a revision record of a rowcolumn insertdelete action.
## RevisionInsertDelete class
Represents a revision record of a row/column insert/delete action.
```javascript
class RevisionInsertDelete extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the inserting/deleting range. |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the action type of this revision. |
| [revisions](#revisions--)| RevisionCollection | Readonly. Gets revision list by this operation. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of revision. |
### constructor(Revision) {#constructor-revision-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Revision);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Revision | The parent object. |
### cellArea {#cellArea--}
Readonly. Gets the inserting/deleting range.
```javascript
cellArea : CellArea;
```
### actionType {#actionType--}
Readonly. Gets the action type of this revision.
```javascript
actionType : RevisionActionType;
```
### revisions {#revisions--}
Readonly. Gets revision list by this operation.
```javascript
revisions : RevisionCollection;
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
Represents the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
