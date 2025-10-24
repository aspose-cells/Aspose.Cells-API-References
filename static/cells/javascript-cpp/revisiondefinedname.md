##RevisionDefinedName
Represents a revision record of a defined name change.
## RevisionDefinedName class
Represents a revision record of a defined name change.
```javascript
class RevisionDefinedName extends Revision;
```
## Constructors
| Name | Description |
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
### getType() {#getType--}
Represents the type of revision.
```javascript
getType() : RevisionType;
```
**Returns**
[RevisionType](../revisiontype/)
