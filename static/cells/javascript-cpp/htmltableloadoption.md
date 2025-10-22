##HtmlTableLoadOption
Represents the option when import table from html.
## HtmlTableLoadOption class
Represents the option when import table from html.
```javascript
class HtmlTableLoadOption;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [tableIndex](#tableIndex--)| number | Get or set the index of table to import from html. |
| [id](#id--)| string | Get or set the id of table to import from html |
| [name](#name--)| string | Get or set the name of table to import from html |
| [originalSheetIndex](#originalSheetIndex--)| number | Get or set the original index of worksheet in the html. |
| [targetSheetIndex](#targetSheetIndex--)| number | Get or set the target index of worksheet where the table is to be located. |
| [tableToListObject](#tableToListObject--)| boolean | Indicates whether generate list objects from imported table. The default value is false. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### tableIndex {#tableIndex--}
Get or set the index of table to import from html.
```javascript
tableIndex : number;
```
### id {#id--}
Get or set the id of table to import from html
```javascript
id : string;
```
### name {#name--}
Get or set the name of table to import from html
```javascript
name : string;
```
### originalSheetIndex {#originalSheetIndex--}
Get or set the original index of worksheet in the html.
```javascript
originalSheetIndex : number;
```
### targetSheetIndex {#targetSheetIndex--}
Get or set the target index of worksheet where the table is to be located.
```javascript
targetSheetIndex : number;
```
### tableToListObject {#tableToListObject--}
Indicates whether generate list objects from imported table. The default value is false.
```javascript
tableToListObject : boolean;
```
