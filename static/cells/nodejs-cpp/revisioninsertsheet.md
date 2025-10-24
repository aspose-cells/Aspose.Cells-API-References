##RevisionInsertSheet
Represents a revision record of a sheet that was inserted.
## RevisionInsertSheet class
Represents a revision record of a sheet that was inserted.
```javascript
class RevisionInsertSheet extends Revision;
```
## Constructors
| Constructor | Description |
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
| [getActionType()](#getActionType--)| <b>@deprecated.</b> Please use the 'actionType' property instead. Gets the action type of the revision. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the worksheet. |
| [getSheetPosition()](#getSheetPosition--)| <b>@deprecated.</b> Please use the 'sheetPosition' property instead. Gets the zero based position of the new sheet in the sheet tab bar. |
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
### getActionType() {#getActionType--}
```javascript
getActionType() : RevisionActionType;
```
**Returns**
[RevisionActionType](../revisionactiontype/)
### getName() {#getName--}
```javascript
getName() : string;
```
### getSheetPosition() {#getSheetPosition--}
```javascript
getSheetPosition() : number;
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
Gets the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
