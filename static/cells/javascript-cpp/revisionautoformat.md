##RevisionAutoFormat
represents a revision record of information about a formatting change.
## RevisionAutoFormat class
represents a revision record of information about a formatting change.
```javascript
class RevisionAutoFormat extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the location where the formatting was applied. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the revision. |
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
Readonly. Gets the location where the formatting was applied.
```javascript
cellArea : CellArea;
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
Gets the type of the revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
