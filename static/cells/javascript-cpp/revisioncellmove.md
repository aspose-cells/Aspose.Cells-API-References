##RevisionCellMove
Represents a revision record on a cells that moved.
## RevisionCellMove class
Represents a revision record on a cell(s) that moved.
```javascript
class RevisionCellMove extends Revision;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [sourceArea](#sourceArea--)| CellArea | Readonly. Gets the source area. |
| [destinationArea](#destinationArea--)| CellArea | Readonly. Gets the destination area. |
| [sourceWorksheet](#sourceWorksheet--)| Worksheet | Readonly. Gets the source worksheet. |
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
### sourceArea {#sourceArea--}
Readonly. Gets the source area.
```javascript
sourceArea : CellArea;
```
### destinationArea {#destinationArea--}
Readonly. Gets the destination area.
```javascript
destinationArea : CellArea;
```
### sourceWorksheet {#sourceWorksheet--}
Readonly. Gets the source worksheet.
```javascript
sourceWorksheet : Worksheet;
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
