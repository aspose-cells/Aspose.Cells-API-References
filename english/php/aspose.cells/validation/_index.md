---
title: "Validation Class"
linktitle: "Validation"
articleTitle: "Validation"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents data validation.settings."
type: docs
weight: 7230
url: /php/aspose.cells/validation/
---

## Validation class

Represents data validation.settings.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Operator](#operator) | Number | Represents the operator for the data validation. The value of the property is OperatorType integer constant. |
| [AlertStyle](#alertstyle) | Number | Represents the validation alert style. The value of the property is ValidationAlertType integer constant. |
| [Type](#type) | Number | Represents the data validation type. The value of the property is ValidationType integer constant. |
| [InputMessage](#inputmessage) | String | Represents the data validation input message. |
| [InputTitle](#inputtitle) | String | Represents the title of the data-validation input dialog box. |
| [ErrorMessage](#errormessage) | String | Represents the data validation error message. |
| [ErrorTitle](#errortitle) | String | Represents the title of the data-validation error dialog box. |
| [ShowInput](#showinput) | boolean | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data valid |
| [ShowError](#showerror) | boolean | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [IgnoreBlank](#ignoreblank) | boolean | Indicates whether blank values are permitted by the range data validation. |
| [Formula1](#formula1) | String | Represents the value or expression associated with the data validation. |
| [Formula2](#formula2) | String | Represents the value or expression associated with the data validation. |
| [Value1](#value1) | Object | Represents the first value associated with the data validation. |
| [Value2](#value2) | Object | Represents the second value associated with the data validation. |
| [InCellDropDown](#incelldropdown) | boolean | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [Areas](#areas) | CellArea[] | Gets all CellArea which contain the data validation settings. |

## Methods

| Name | Description |
| --- | --- |
| [getFormula1](#getformula1) | Gets the value or expression associated with this validation. |
| [getFormula2](#getformula2) | Gets the value or expression associated with this validation. |
| [setFormula1](#setformula1) | Sets the value or expression associated with this validation. |
| [setFormula2](#setformula2) | Sets the value or expression associated with this validation. |
| [getListValue](#getlistvalue) | Get the value for list of the validation for the specified cell.

Only for validation whose type is List and has been ap |
| [getValue](#getvalue) | Get the value of validation on the specific cell. |
| [addArea](#addarea) | Applies the validation to the area.

It is equivalent to use addArea(com.aspose.cells.CellArea, boolean, boolean) with c |
| [addAreas](#addareas) | Applies the validation to given areas.

In this method, we will remove all old validations in given area. For the top-le |
| [removeArea](#removearea) | Remove the validation settings in the range. |
| [removeAreas](#removeareas) | Removes this validation from given areas. |
| [removeACell](#removeacell) | Remove the validation settings in the cell. |
| [copy](#copy) | Copy validation. |

### Validation.Operator property {#operator}

Represents the operator for the data validation. The value of the property is OperatorType integer constant.

**Type:** Number

### Validation.AlertStyle property {#alertstyle}

Represents the validation alert style. The value of the property is ValidationAlertType integer constant.

**Type:** Number

### Validation.Type property {#type}

Represents the data validation type. The value of the property is ValidationType integer constant.

**Type:** Number

### Validation.InputMessage property {#inputmessage}

Represents the data validation input message.

**Type:** String

### Validation.InputTitle property {#inputtitle}

Represents the title of the data-validation input dialog box.

**Type:** String

### Validation.ErrorMessage property {#errormessage}

Represents the data validation error message.

**Type:** String

### Validation.ErrorTitle property {#errortitle}

Represents the title of the data-validation error dialog box.

**Type:** String

### Validation.ShowInput property {#showinput}

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

**Type:** boolean

### Validation.ShowError property {#showerror}

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

**Type:** boolean

### Validation.IgnoreBlank property {#ignoreblank}

Indicates whether blank values are permitted by the range data validation.

**Type:** boolean

### Validation.Formula1 property {#formula1}

Represents the value or expression associated with the data validation.

**Type:** String

### Validation.Formula2 property {#formula2}

Represents the value or expression associated with the data validation.

**Type:** String

### Validation.Value1 property {#value1}

Represents the first value associated with the data validation.

**Type:** Object

### Validation.Value2 property {#value2}

Represents the second value associated with the data validation.

**Type:** Object

### Validation.InCellDropDown property {#incelldropdown}

Indicates whether data validation displays a drop-down list that contains acceptable values.

**Type:** boolean

### Validation.Areas property {#areas}

Gets all CellArea which contain the data validation settings.

**Type:** CellArea[]

### getFormula1(isR1C1, isLocal) (1 of 2) {#getformula1}

Gets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The value or expression associated with this validation.

---

### getFormula1(isR1C1, isLocal, row, column) (2 of 2) {#getformula1-1}

Gets the value or expression associated with this validation for specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** The value or expression associated with this validation.

### getFormula2(isR1C1, isLocal) (1 of 2) {#getformula2}

Gets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The value or expression associated with this validation.

---

### getFormula2(isR1C1, isLocal, row, column) (2 of 2) {#getformula2-1}

Gets the value or expression associated with this validation for specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** The value or expression associated with this validation.

### setFormula1(formula, isR1C1, isLocal) {#setformula1}

Sets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2(formula, isR1C1, isLocal) {#setformula2}

Sets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### getListValue(row, column) {#getlistvalue}

Get the value for list of the validation for the specified cell.

Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a ReferredArea object; Otherwise the returned value may be null, object[], or simple object.

### getValue(row, column, isValue1) {#getvalue}

Get the value of validation on the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |
| isValue1 | boolean | Indicates whether getting the first value. |

### addArea(cellArea) (1 of 2) {#addarea}

Applies the validation to the area.

It is equivalent to use addArea(com.aspose.cells.CellArea, boolean, boolean) with checking intersection and edge.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |

---

### addArea(cellArea, checkIntersection, checkEdge) (2 of 2) {#addarea-1}

Applies the validation to the area.

In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that the added area does not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if given area will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that the added area is not the top-left one, this parameter can be set as false for performance consideration. |

### addAreas(areas, checkIntersection, checkEdge) {#addareas}

Applies the validation to given areas.

In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

| Parameter | Type | Description |
| --- | --- | --- |
| areas | CellArea[] | The areas. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |

### removeArea(cellArea) {#removearea}

Remove the validation settings in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | the areas where this validation settings should be removed. |

### removeAreas(areas) {#removeareas}

Removes this validation from given areas.

| Parameter | Type | Description |
| --- | --- | --- |
| areas | CellArea[] | the areas where this validation settings should be removed. |

### removeACell(row, column) {#removeacell}

Remove the validation settings in the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

### copy(source, copyOption) {#copy}

Copy validation.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Validation | The source validation. |
| copyOption | CopyOptions | The copy option. |
