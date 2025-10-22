##RevisionQueryTable
Represents a revision of a query table field change.
## RevisionQueryTable class
Represents a revision of a query table field change.
```javascript
class RevisionQueryTable extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the location of the affected query table. |
| [fieldId](#fieldId--)| number | Readonly. Gets ID of the specific query table field that was removed. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
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
### cellArea {#cellArea--}
Readonly. Gets the location of the affected query table.
```javascript
cellArea : CellArea;
```
### fieldId {#fieldId--}
Readonly. Gets ID of the specific query table field that was removed.
```javascript
fieldId : number;
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
Represents the type of the revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
