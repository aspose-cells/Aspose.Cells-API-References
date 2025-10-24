##RevisionFormat
Represents a revision record of information about a formatting change.
## RevisionFormat class
Represents a revision record of information about a formatting change.
```javascript
class RevisionFormat extends Revision;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [areas](#areas--)| CellArea[] | Readonly. The range to which this formatting was applied. |
| [style](#style--)| Style | Readonly. Gets the applied style. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getAreas()](#getAreas--)| <b>@deprecated.</b> Please use the 'areas' property instead. The range to which this formatting was applied. |
| [getStyle()](#getStyle--)| <b>@deprecated.</b> Please use the 'style' property instead. Gets the applied style. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the worksheet. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the number of this revision. |
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
### areas {#areas--}
Readonly. The range to which this formatting was applied.
```javascript
areas : CellArea[];
```
### style {#style--}
Readonly. Gets the applied style.
```javascript
style : Style;
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
### getAreas() {#getAreas--}
```javascript
getAreas() : CellArea[];
```
**Returns**
[CellArea](../cellarea/)[]
### getStyle() {#getStyle--}
```javascript
getStyle() : Style;
```
**Returns**
[Style](../style/)
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
Gets the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
