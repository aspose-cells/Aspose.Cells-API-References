##RevisionDefinedName
Represents a revision record of a defined name change.
## RevisionDefinedName class
Represents a revision record of a defined name change.
```javascript
class RevisionDefinedName extends Revision;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [text](#text--)| string | Readonly. Gets the text of the defined name. |
| [oldFormula](#oldFormula--)| string | Readonly. Gets the old formula. |
| [newFormula](#newFormula--)| string | Readonly. Gets the formula. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |
## Methods
| Method | Description |
| --- | --- |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Gets the text of the defined name. |
| [getOldFormula()](#getOldFormula--)| <b>@deprecated.</b> Please use the 'oldFormula' property instead. Gets the old formula. |
| [getNewFormula()](#getNewFormula--)| <b>@deprecated.</b> Please use the 'newFormula' property instead. Gets the formula. |
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
### text {#text--}
Readonly. Gets the text of the defined name.
```javascript
text : string;
```
### oldFormula {#oldFormula--}
Readonly. Gets the old formula.
```javascript
oldFormula : string;
```
### newFormula {#newFormula--}
Readonly. Gets the formula.
```javascript
newFormula : string;
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
### getText() {#getText--}
```javascript
getText() : string;
```
### getOldFormula() {#getOldFormula--}
```javascript
getOldFormula() : string;
```
### getNewFormula() {#getNewFormula--}
```javascript
getNewFormula() : string;
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
Represents the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
