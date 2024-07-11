---
title: Validation
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents data validation.settings.
type: docs
url: /nodejs-cpp/validation/
---

## Validation class

Represents data validation.settings.

```javascript
class Validation;
```


## Methods

| Method | Description |
| --- | --- |
| [getOperator()](#getOperator--)| Represents the operator for the data validation. |
| [setOperator(OperatorType)](#setOperator-operatortype-)| Represents the operator for the data validation. |
| [getAlertStyle()](#getAlertStyle--)| Represents the validation alert style. |
| [setAlertStyle(ValidationAlertType)](#setAlertStyle-validationalerttype-)| Represents the validation alert style. |
| [getType()](#getType--)| Represents the data validation type. |
| [setType(ValidationType)](#setType-validationtype-)| Represents the data validation type. |
| [getInputMessage()](#getInputMessage--)| Represents the data validation input message. |
| [setInputMessage(string)](#setInputMessage-string-)| Represents the data validation input message. |
| [getInputTitle()](#getInputTitle--)| Represents the title of the data-validation input dialog box. |
| [setInputTitle(string)](#setInputTitle-string-)| Represents the title of the data-validation input dialog box. |
| [getErrorMessage()](#getErrorMessage--)| Represents the data validation error message. |
| [setErrorMessage(string)](#setErrorMessage-string-)| Represents the data validation error message. |
| [getErrorTitle()](#getErrorTitle--)| Represents the title of the data-validation error dialog box. |
| [setErrorTitle(string)](#setErrorTitle-string-)| Represents the title of the data-validation error dialog box. |
| [getShowInput()](#getShowInput--)| Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [setShowInput(boolean)](#setShowInput-boolean-)| Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [getShowError()](#getShowError--)| Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [setShowError(boolean)](#setShowError-boolean-)| Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [getIgnoreBlank()](#getIgnoreBlank--)| Indicates whether blank values are permitted by the range data validation. |
| [setIgnoreBlank(boolean)](#setIgnoreBlank-boolean-)| Indicates whether blank values are permitted by the range data validation. |
| [getInCellDropDown()](#getInCellDropDown--)| Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [setInCellDropDown(boolean)](#setInCellDropDown-boolean-)| Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [getAreas()](#getAreas--)| Gets all [CellArea](./cellarea/) which contain the data validation settings. |
| [getFormula1(boolean, boolean)](#getFormula1-boolean-boolean-)| Gets the value or expression associated with this validation. |
| [getFormula1(boolean, boolean, number, number)](#getFormula1-boolean-boolean-number-number-)| Gets the value or expression associated with this validation for specific cell. |
| [getFormula2(boolean, boolean)](#getFormula2-boolean-boolean-)| Gets the value or expression associated with this validation. |
| [getFormula2(boolean, boolean, number, number)](#getFormula2-boolean-boolean-number-number-)| Gets the value or expression associated with this validation for specific cell. |
| [setFormula1(string, boolean, boolean)](#setFormula1-string-boolean-boolean-)| Sets the value or expression associated with this validation. |
| [setFormula2(string, boolean, boolean)](#setFormula2-string-boolean-boolean-)| Sets the value or expression associated with this validation. |
| [addArea(CellArea)](#addArea-cellarea-)| Applies the validation to the area. |
| [addArea(CellArea, boolean, boolean)](#addArea-cellarea-boolean-boolean-)| Applies the validation to the area. |
| [addAreas(CellArea[], boolean, boolean)](#addAreas-cellarea[]-boolean-boolean-)| Applies the validation to given areas. |
| [removeArea(CellArea)](#removeArea-cellarea-)| Remove the validation settings in the range. |
| [removeAreas(CellArea[])](#removeAreas-cellarea[]-)| Removes this validation from given areas. |
| [removeACell(number, number)](#removeACell-number-number-)| Remove the validation settings in the cell. |
| [copy(Validation, CopyOptions)](#copy-validation-copyoptions-)| Copy validation. |


### getOperator() {#getOperator--}

Represents the operator for the data validation.

```javascript
getOperator() : OperatorType;
```


**Returns**

[OperatorType](./operatortype/)

### setOperator(OperatorType) {#setOperator-operatortype-}

Represents the operator for the data validation.

```javascript
setOperator(value: OperatorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OperatorType](./operatortype/) | The value to set. |

### getAlertStyle() {#getAlertStyle--}

Represents the validation alert style.

```javascript
getAlertStyle() : ValidationAlertType;
```


**Returns**

[ValidationAlertType](./validationalerttype/)

### setAlertStyle(ValidationAlertType) {#setAlertStyle-validationalerttype-}

Represents the validation alert style.

```javascript
setAlertStyle(value: ValidationAlertType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ValidationAlertType](./validationalerttype/) | The value to set. |

### getType() {#getType--}

Represents the data validation type.

```javascript
getType() : ValidationType;
```


**Returns**

[ValidationType](./validationtype/)

### setType(ValidationType) {#setType-validationtype-}

Represents the data validation type.

```javascript
setType(value: ValidationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ValidationType](./validationtype/) | The value to set. |

### getInputMessage() {#getInputMessage--}

Represents the data validation input message.

```javascript
getInputMessage() : string;
```


### setInputMessage(string) {#setInputMessage-string-}

Represents the data validation input message.

```javascript
setInputMessage(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getInputTitle() {#getInputTitle--}

Represents the title of the data-validation input dialog box.

```javascript
getInputTitle() : string;
```


### setInputTitle(string) {#setInputTitle-string-}

Represents the title of the data-validation input dialog box.

```javascript
setInputTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getErrorMessage() {#getErrorMessage--}

Represents the data validation error message.

```javascript
getErrorMessage() : string;
```


### setErrorMessage(string) {#setErrorMessage-string-}

Represents the data validation error message.

```javascript
setErrorMessage(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getErrorTitle() {#getErrorTitle--}

Represents the title of the data-validation error dialog box.

```javascript
getErrorTitle() : string;
```


### setErrorTitle(string) {#setErrorTitle-string-}

Represents the title of the data-validation error dialog box.

```javascript
setErrorTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getShowInput() {#getShowInput--}

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

```javascript
getShowInput() : boolean;
```


### setShowInput(boolean) {#setShowInput-boolean-}

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

```javascript
setShowInput(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowError() {#getShowError--}

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

```javascript
getShowError() : boolean;
```


### setShowError(boolean) {#setShowError-boolean-}

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

```javascript
setShowError(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreBlank() {#getIgnoreBlank--}

Indicates whether blank values are permitted by the range data validation.

```javascript
getIgnoreBlank() : boolean;
```


### setIgnoreBlank(boolean) {#setIgnoreBlank-boolean-}

Indicates whether blank values are permitted by the range data validation.

```javascript
setIgnoreBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getInCellDropDown() {#getInCellDropDown--}

Indicates whether data validation displays a drop-down list that contains acceptable values.

```javascript
getInCellDropDown() : boolean;
```


### setInCellDropDown(boolean) {#setInCellDropDown-boolean-}

Indicates whether data validation displays a drop-down list that contains acceptable values.

```javascript
setInCellDropDown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAreas() {#getAreas--}

Gets all [CellArea](./cellarea/) which contain the data validation settings.

```javascript
getAreas() : CellArea[];
```


**Returns**

[CellArea](./cellarea/)[]

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

### addArea(CellArea) {#addArea-cellarea-}

Applies the validation to the area.

```javascript
addArea(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](./cellarea/) | The area. |

**Remarks**

It is equivalent to use [AddArea(Aspose.Cells.CellArea,bool,bool)](./addarea(aspose.cells.cellarea,bool,bool)/) with checking intersection and edge.

### addArea(CellArea, boolean, boolean) {#addArea-cellarea-boolean-boolean-}

Applies the validation to the area.

```javascript
addArea(cellArea: CellArea, checkIntersection: boolean, checkEdge: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](./cellarea/) | The area. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas.         /// If one validation has been applied in given area(or part of it),         /// then the existing validation should be removed at first from given area.         /// Otherwise corruption may be caused for the generated Validations.         /// If user is sure that the added area does not intersect with any existing area,         /// this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas.         /// Validation's internal settings depend on the top-left one of its applied ranges,         /// so if given area will become the new top-left one of the applied ranges,         /// the internal settings should be changed and rebuilt, otherwise unexpected result may be caused.         /// If user is sure that the added area is not the top-left one,         /// this parameter can be set as false for performance consideration. |

**Remarks**

In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

### addAreas(CellArea[], boolean, boolean) {#addAreas-cellarea[]-boolean-boolean-}

Applies the validation to given areas.

```javascript
addAreas(areas: CellArea[], checkIntersection: boolean, checkEdge: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea](./cellarea/)[] | The areas. |
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
| cellArea | [CellArea](./cellarea/) | the areas where this validation settings should be removed. |

### removeAreas(CellArea[]) {#removeAreas-cellarea[]-}

Removes this validation from given areas.

```javascript
removeAreas(areas: CellArea[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea](./cellarea/)[] | the areas where this validation settings should be removed. |

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
| source | [Validation](./validation/) | The source validation. |
| copyOption | [CopyOptions](./copyoptions/) | The copy option. |


