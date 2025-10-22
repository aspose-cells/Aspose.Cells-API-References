##Validation
Represents data validation.settings.
## Validation class
Represents data validation.settings.
```javascript
class Validation;
```
### Example
```javascript
const { Workbook, ValidationType, CellArea } = AsposeCells;
var workbook = new Workbook();
var validations = workbook.worksheets.get(0).validations;
var area = CellArea.createCellArea(0, 0, 1, 1);
var validation = validations.get(validations.add(area));
validation.type = ValidationType.List;
validation.formula1 = "a,b,c,d";
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [operator](#operator--)| OperatorType | Represents the operator for the data validation. |
| [alertStyle](#alertStyle--)| ValidationAlertType | Represents the validation alert style. |
| [type](#type--)| ValidationType | Represents the data validation type. |
| [inputMessage](#inputMessage--)| string | Represents the data validation input message. |
| [inputTitle](#inputTitle--)| string | Represents the title of the data-validation input dialog box. |
| [errorMessage](#errorMessage--)| string | Represents the data validation error message. |
| [errorTitle](#errorTitle--)| string | Represents the title of the data-validation error dialog box. |
| [showInput](#showInput--)| boolean | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [showError](#showError--)| boolean | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [ignoreBlank](#ignoreBlank--)| boolean | Indicates whether blank values are permitted by the range data validation. |
| [formula1](#formula1--)| string | Represents the value or expression associated with the data validation. |
| [formula2](#formula2--)| string | Represents the value or expression associated with the data validation. |
| [value1](#value1--)| VObject | Represents the first value associated with the data validation. |
| [value2](#value2--)| VObject | Represents the second value associated with the data validation. |
| [inCellDropDown](#inCellDropDown--)| boolean | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [areas](#areas--)| CellArea[] | Readonly. Gets all [CellArea](../cellarea/) which contain the data validation settings. |
## Methods
| Method | Description |
| --- | --- |
| [getFormula1(boolean, boolean)](#getFormula1-boolean-boolean-)| Gets the value or expression associated with this validation. |
| [getFormula1(boolean, boolean, number, number)](#getFormula1-boolean-boolean-number-number-)| Gets the value or expression associated with this validation for specific cell. |
| [getFormula2(boolean, boolean)](#getFormula2-boolean-boolean-)| Gets the value or expression associated with this validation. |
| [getFormula2(boolean, boolean, number, number)](#getFormula2-boolean-boolean-number-number-)| Gets the value or expression associated with this validation for specific cell. |
| [setFormula1(string, boolean, boolean)](#setFormula1-string-boolean-boolean-)| Sets the value or expression associated with this validation. |
| [setFormula2(string, boolean, boolean)](#setFormula2-string-boolean-boolean-)| Sets the value or expression associated with this validation. |
| [getListValue(number, number)](#getListValue-number-number-)| Get the value for list of the validation for the specified cell. |
| [getValue(number, number, boolean)](#getValue-number-number-boolean-)| Get the value of validation on the specific cell. |
| [addArea(CellArea)](#addArea-cellarea-)| Applies the validation to the area. |
| [addArea(CellArea, boolean, boolean)](#addArea-cellarea-boolean-boolean-)| Applies the validation to the area. |
| [addAreas(CellArea[], boolean, boolean)](#addAreas-cellareaarray-boolean-boolean-)| Applies the validation to given areas. |
| [removeArea(CellArea)](#removeArea-cellarea-)| Remove the validation settings in the range. |
| [removeAreas(CellArea[])](#removeAreas-cellareaarray-)| Removes this validation from given areas. |
| [removeACell(number, number)](#removeACell-number-number-)| Remove the validation settings in the cell. |
| [copy(Validation, CopyOptions)](#copy-validation-copyoptions-)| Copy validation. |
### operator {#operator--}
Represents the operator for the data validation.
```javascript
operator : OperatorType;
```
### alertStyle {#alertStyle--}
Represents the validation alert style.
```javascript
alertStyle : ValidationAlertType;
```
### type {#type--}
Represents the data validation type.
```javascript
type : ValidationType;
```
### inputMessage {#inputMessage--}
Represents the data validation input message.
```javascript
inputMessage : string;
```
### inputTitle {#inputTitle--}
Represents the title of the data-validation input dialog box.
```javascript
inputTitle : string;
```
### errorMessage {#errorMessage--}
Represents the data validation error message.
```javascript
errorMessage : string;
```
### errorTitle {#errorTitle--}
Represents the title of the data-validation error dialog box.
```javascript
errorTitle : string;
```
### showInput {#showInput--}
Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.
```javascript
showInput : boolean;
```
### showError {#showError--}
Indicates whether the data validation error message will be displayed whenever the user enters invalid data.
```javascript
showError : boolean;
```
### ignoreBlank {#ignoreBlank--}
Indicates whether blank values are permitted by the range data validation.
```javascript
ignoreBlank : boolean;
```
### formula1 {#formula1--}
Represents the value or expression associated with the data validation.
```javascript
formula1 : string;
```
### formula2 {#formula2--}
Represents the value or expression associated with the data validation.
```javascript
formula2 : string;
```
### value1 {#value1--}
Represents the first value associated with the data validation.
```javascript
value1 : VObject;
```
### value2 {#value2--}
Represents the second value associated with the data validation.
```javascript
value2 : VObject;
```
### inCellDropDown {#inCellDropDown--}
Indicates whether data validation displays a drop-down list that contains acceptable values.
```javascript
inCellDropDown : boolean;
```
### areas {#areas--}
Readonly. Gets all [CellArea](../cellarea/) which contain the data validation settings.
```javascript
areas : CellArea[];
```
### getFormula1(boolean, boolean) {#getFormula1-boolean-boolean-}
Gets the value or expression associated with this validation.
```javascript
getFormula1(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The value or expression associated with this validation.
### getFormula1(boolean, boolean, number, number) {#getFormula1-boolean-boolean-number-number-}
Gets the value or expression associated with this validation for specific cell.
```javascript
getFormula1(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The value or expression associated with this validation.
### getFormula2(boolean, boolean) {#getFormula2-boolean-boolean-}
Gets the value or expression associated with this validation.
```javascript
getFormula2(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The value or expression associated with this validation.
### getFormula2(boolean, boolean, number, number) {#getFormula2-boolean-boolean-number-number-}
Gets the value or expression associated with this validation for specific cell.
```javascript
getFormula2(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The value or expression associated with this validation.
### setFormula1(string, boolean, boolean) {#setFormula1-string-boolean-boolean-}
Sets the value or expression associated with this validation.
```javascript
setFormula1(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### setFormula2(string, boolean, boolean) {#setFormula2-string-boolean-boolean-}
Sets the value or expression associated with this validation.
```javascript
setFormula2(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### getListValue(number, number) {#getListValue-number-number-}
Get the value for list of the validation for the specified cell.
```javascript
getListValue(row: number, column: number) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [ReferredArea](../referredarea/) object; Otherwise the returned value may be null, object[], or simple object.
**Remarks**
Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.
### getValue(number, number, boolean) {#getValue-number-number-boolean-}
Get the value of validation on the specific cell.
```javascript
getValue(row: number, column: number, isValue1: boolean) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
| isValue1 | boolean | Indicates whether getting the first value. |
### addArea(CellArea) {#addArea-cellarea-}
Applies the validation to the area.
```javascript
addArea(cellArea: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | The area. |
**Remarks**
It is equivalent to use [AddArea(Aspose.Cells.CellArea,bool,bool)](../addarea(aspose.cells.cellarea,bool,bool)/) with checking intersection and edge.
### addArea(CellArea, boolean, boolean) {#addArea-cellarea-boolean-boolean-}
Applies the validation to the area.
```javascript
addArea(cellArea: CellArea, checkIntersection: boolean, checkEdge: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | The area. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas.         /// If one validation has been applied in given area(or part of it),         /// then the existing validation should be removed at first from given area.         /// Otherwise corruption may be caused for the generated Validations.         /// If user is sure that the added area does not intersect with any existing area,         /// this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas.         /// Validation's internal settings depend on the top-left one of its applied ranges,         /// so if given area will become the new top-left one of the applied ranges,         /// the internal settings should be changed and rebuilt, otherwise unexpected result may be caused.         /// If user is sure that the added area is not the top-left one,         /// this parameter can be set as false for performance consideration. |
**Remarks**
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### addAreas(CellArea[], boolean, boolean) {#addAreas-cellareaarray-boolean-boolean-}
Applies the validation to given areas.
```javascript
addAreas(areas: CellArea[], checkIntersection: boolean, checkEdge: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea](../cellarea/)[] | The areas. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas.         /// If one validation has been applied in given area(or part of it),         /// then the existing validation should be removed at first from given area.         /// Otherwise corruption may be caused for the generated Validations.         /// If user is sure that all the added areas do not intersect with any existing area,         /// this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas.         /// Validation's internal settings depend on the top-left one of its applied ranges,         /// so if one of given areas will become the new top-left one of the applied ranges,         /// the internal settings should be changed and rebuilt, otherwise unexpected result may be caused.         /// If user is sure that no one of those added areas is the top-left,         /// this parameter can be set as false for performance consideration. |
**Remarks**
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### removeArea(CellArea) {#removeArea-cellarea-}
Remove the validation settings in the range.
```javascript
removeArea(cellArea: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | the areas where this validation settings should be removed. |
### removeAreas(CellArea[]) {#removeAreas-cellareaarray-}
Removes this validation from given areas.
```javascript
removeAreas(areas: CellArea[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea](../cellarea/)[] | the areas where this validation settings should be removed. |
### removeACell(number, number) {#removeACell-number-number-}
Remove the validation settings in the cell.
```javascript
removeACell(row: number, column: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
### copy(Validation, CopyOptions) {#copy-validation-copyoptions-}
Copy validation.
```javascript
copy(source: Validation, copyOption: CopyOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Validation](../validation/) | The source validation. |
| copyOption | [CopyOptions](../copyoptions/) | The copy option. |
