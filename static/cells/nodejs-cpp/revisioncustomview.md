##RevisionCustomView
Represents a revision record of adding or removing a custom view to the workbook
## RevisionCustomView class
Represents a revision record of adding or removing a custom view to the workbook
```javascript
class RevisionCustomView extends Revision;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the type of action. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getActionType()](#getActionType--)| <b>@deprecated.</b> Please use the 'actionType' property instead. Gets the type of action. |
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
Readonly. Gets the type of action.
```javascript
actionType : RevisionActionType;
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
