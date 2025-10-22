##RevisionCellChange
Represents the revision that changing cells.
## RevisionCellChange class
Represents the revision that changing cells.
```javascript
class RevisionCellChange extends Revision;
```
## Constructors
| Name | Description |
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
| [oldValue](#oldValue--)| VObject | Readonly. Gets old value of the cell. |
| [newValue](#newValue--)| VObject | Readonly. Gets new value of the cell. |
| [newFormula](#newFormula--)| string | Readonly. Gets the old formula. |
| [newStyle](#newStyle--)| Style | Readonly. Gets the new style of the cell. |
| [oldStyle](#oldStyle--)| Style | Readonly. Gets the old style of the cell. |
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
oldValue : VObject;
```
### newValue {#newValue--}
Readonly. Gets new value of the cell.
```javascript
newValue : VObject;
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
### getType() {#getType--}
Represents the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
