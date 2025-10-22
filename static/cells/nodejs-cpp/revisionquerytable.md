##RevisionQueryTable
Represents a revision of a query table field change.
## RevisionQueryTable class
Represents a revision of a query table field change.
```javascript
class RevisionQueryTable extends Revision;
```
## Constructors
| Constructor | Description |
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
| [getCellArea()](#getCellArea--)| <b>@deprecated.</b> Please use the 'cellArea' property instead. Gets the location of the affected query table. |
| [getFieldId()](#getFieldId--)| <b>@deprecated.</b> Please use the 'fieldId' property instead. Gets ID of the specific query table field that was removed. |
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
### getCellArea() {#getCellArea--}
```javascript
getCellArea() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getFieldId() {#getFieldId--}
```javascript
getFieldId() : number;
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
