##RevisionCellComment
Represents a revision record of a cell comment change.
## RevisionCellComment class
Represents a revision record of a cell comment change.
```javascript
class RevisionCellComment extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [row](#row--)| number | Readonly. Gets the row index of the which contains a comment. |
| [column](#column--)| number | Readonly. Gets the column index of the which contains a comment. |
| [cellName](#cellName--)| string | Gets the name of the cell. |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the action type of the revision. |
| [isOldComment](#isOldComment--)| boolean | Readonly. Indicates whether it's an  old comment. |
| [oldLength](#oldLength--)| number | Readonly. Gets Length of the comment text added in this revision. |
| [newLength](#newLength--)| number | Readonly. Gets Length of the comment before this revision was made. |
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
### row {#row--}
Readonly. Gets the row index of the which contains a comment.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column index of the which contains a comment.
```javascript
column : number;
```
### cellName {#cellName--}
Gets the name of the cell.
```javascript
cellName : string;
```
### actionType {#actionType--}
Readonly. Gets the action type of the revision.
```javascript
actionType : RevisionActionType;
```
### isOldComment {#isOldComment--}
Readonly. Indicates whether it's an  old comment.
```javascript
isOldComment : boolean;
```
### oldLength {#oldLength--}
Readonly. Gets Length of the comment text added in this revision.
```javascript
oldLength : number;
```
### newLength {#newLength--}
Readonly. Gets Length of the comment before this revision was made.
```javascript
newLength : number;
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
