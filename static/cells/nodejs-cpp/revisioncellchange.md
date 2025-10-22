##RevisionCellChange
Represents the revision that changing cells.
## RevisionCellChange class
Represents the revision that changing cells.
```javascript
class RevisionCellChange extends Revision;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cellName](#cellName--)| string | Readonly. Gets the name of the cell. |
| [row](#row--)| number | Readonly. Gets the row index of the cell. |
| [column](#column--)| number | Readonly. Gets the column index of the cell. |
| [isNewFormatted](#isNewFormatted--)| boolean | Readonly. Indicates whether this cell is new formatted. |
| [isOldFormatted](#isOldFormatted--)| boolean | Readonly. Indicates whether this cell is old formatted. |
| [oldFormula](#oldFormula--)| string | Readonly. Gets the old formula. |
| [oldValue](#oldValue--)| Object | Readonly. Gets old value of the cell. |
| [newValue](#newValue--)| Object | Readonly. Gets new value of the cell. |
| [newFormula](#newFormula--)| string | Readonly. Gets the old formula. |
| [newStyle](#newStyle--)| Style | Readonly. Gets the new style of the cell. |
| [oldStyle](#oldStyle--)| Style | Readonly. Gets the old style of the cell. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getCellName()](#getCellName--)| <b>@deprecated.</b> Please use the 'cellName' property instead. Gets the name of the cell. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the cell. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the cell. |
| [isNewFormatted()](#isNewFormatted--)| <b>@deprecated.</b> Please use the 'isNewFormatted' property instead. Indicates whether this cell is new formatted. |
| [isOldFormatted()](#isOldFormatted--)| <b>@deprecated.</b> Please use the 'isOldFormatted' property instead. Indicates whether this cell is old formatted. |
| [getOldFormula()](#getOldFormula--)| <b>@deprecated.</b> Please use the 'oldFormula' property instead. Gets the old formula. |
| [getOldValue()](#getOldValue--)| <b>@deprecated.</b> Please use the 'oldValue' property instead. Gets old value of the cell. |
| [getNewValue()](#getNewValue--)| <b>@deprecated.</b> Please use the 'newValue' property instead. Gets new value of the cell. |
| [getNewFormula()](#getNewFormula--)| <b>@deprecated.</b> Please use the 'newFormula' property instead. Gets the old formula. |
| [getNewStyle()](#getNewStyle--)| <b>@deprecated.</b> Please use the 'newStyle' property instead. Gets the new style of the cell. |
| [getOldStyle()](#getOldStyle--)| <b>@deprecated.</b> Please use the 'oldStyle' property instead. Gets the old style of the cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the worksheet. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the number of this revision. |
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
### cellName {#cellName--}
Readonly. Gets the name of the cell.
```javascript
cellName : string;
```
### row {#row--}
Readonly. Gets the row index of the cell.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column index of the cell.
```javascript
column : number;
```
### isNewFormatted {#isNewFormatted--}
Readonly. Indicates whether this cell is new formatted.
```javascript
isNewFormatted : boolean;
```
### isOldFormatted {#isOldFormatted--}
Readonly. Indicates whether this cell is old formatted.
```javascript
isOldFormatted : boolean;
```
### oldFormula {#oldFormula--}
Readonly. Gets the old formula.
```javascript
oldFormula : string;
```
### oldValue {#oldValue--}
Readonly. Gets old value of the cell.
```javascript
oldValue : Object;
```
### newValue {#newValue--}
Readonly. Gets new value of the cell.
```javascript
newValue : Object;
```
### newFormula {#newFormula--}
Readonly. Gets the old formula.
```javascript
newFormula : string;
```
### newStyle {#newStyle--}
Readonly. Gets the new style of the cell.
```javascript
newStyle : Style;
```
### oldStyle {#oldStyle--}
Readonly. Gets the old style of the cell.
```javascript
oldStyle : Style;
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
### getCellName() {#getCellName--}
```javascript
getCellName() : string;
```
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### isNewFormatted() {#isNewFormatted--}
```javascript
isNewFormatted() : boolean;
```
### isOldFormatted() {#isOldFormatted--}
```javascript
isOldFormatted() : boolean;
```
### getOldFormula() {#getOldFormula--}
```javascript
getOldFormula() : string;
```
### getOldValue() {#getOldValue--}
```javascript
getOldValue() : Object;
```
### getNewValue() {#getNewValue--}
```javascript
getNewValue() : Object;
```
### getNewFormula() {#getNewFormula--}
```javascript
getNewFormula() : string;
```
### getNewStyle() {#getNewStyle--}
```javascript
getNewStyle() : Style;
```
**Returns**
[Style](../style/)
### getOldStyle() {#getOldStyle--}
```javascript
getOldStyle() : Style;
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
Represents the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
