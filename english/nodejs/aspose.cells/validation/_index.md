---
title: "Validation"
linktitle: "Validation"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents data validation.settings."
type: docs
weight: 4440
url: /nodejs/aspose.cells/validation/
---

## Validation class

Represents data validation.settings.

## Methods

| Name | Description |
| --- | --- |
| [addArea(cellArea)](#addarea) | Applies the validation to the area. It is equivalent to use addArea(com.aspose.cells.CellArea, boolean, boolean) with ch |
| [addArea(cellArea, checkIntersection, checkEdge)](#addarea-1) | Applies the validation to the area. In this method, we will remove all old validations in given area. For the top-left o |
| [addAreas(areas, checkIntersection, checkEdge)](#addareas) | Applies the validation to given areas. In this method, we will remove all old validations in given area. For the top-lef |
| [copy(source, copyOption)](#copy) | Copy validation. |
| [getAlertStyle()](#getalertstyle) | Represents the validation alert style. The value of the property is ValidationAlertType integer constant. |
| [getAreas()](#getareas) | Gets all CellArea which contain the data validation settings. |
| [getErrorMessage()](#geterrormessage) | Represents the data validation error message. |
| [getErrorTitle()](#geterrortitle) | Represents the title of the data-validation error dialog box. |
| [getFormula1()](#getformula1) | Represents the value or expression associated with the data validation. |
| [getFormula1(isR1C1, isLocal)](#getformula1-1) | Gets the value or expression associated with this validation. |
| [getFormula1(isR1C1, isLocal, row, column)](#getformula1-2) | Gets the value or expression associated with this validation for specific cell. |
| [getFormula2()](#getformula2) | Represents the value or expression associated with the data validation. |
| [getFormula2(isR1C1, isLocal)](#getformula2-1) | Gets the value or expression associated with this validation. |
| [getFormula2(isR1C1, isLocal, row, column)](#getformula2-2) | Gets the value or expression associated with this validation for specific cell. |
| [getIgnoreBlank()](#getignoreblank) | Indicates whether blank values are permitted by the range data validation. |
| [getInCellDropDown()](#getincelldropdown) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [getInputMessage()](#getinputmessage) | Represents the data validation input message. |
| [getInputTitle()](#getinputtitle) | Represents the title of the data-validation input dialog box. |
| [getListValue(row, column)](#getlistvalue) | Get the value for list of the validation for the specified cell. Only for validation whose type is List and has been app |
| [getOperator()](#getoperator) | Represents the operator for the data validation. The value of the property is OperatorType integer constant. |
| [getShowError()](#getshowerror) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [getShowInput()](#getshowinput) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data valid |
| [getType()](#gettype) | Represents the data validation type. The value of the property is ValidationType integer constant. |
| [getValue(row, column, isValue1)](#getvalue) | Get the value of validation on the specific cell. |
| [getValue1()](#getvalue1) | Represents the first value associated with the data validation. |
| [getValue2()](#getvalue2) | Represents the second value associated with the data validation. |
| [removeACell(row, column)](#removeacell) | Remove the validation settings in the cell. |
| [removeArea(cellArea)](#removearea) | Remove the validation settings in the range. |
| [removeAreas(areas)](#removeareas) | Removes this validation from given areas. |
| [setAlertStyle()](#setalertstyle) | Represents the validation alert style. The value of the property is ValidationAlertType integer constant. |
| [setErrorMessage()](#seterrormessage) | Represents the data validation error message. |
| [setErrorTitle()](#seterrortitle) | Represents the title of the data-validation error dialog box. |
| [setFormula1()](#setformula1) | Represents the value or expression associated with the data validation. |
| [setFormula1(formula, isR1C1, isLocal)](#setformula1-1) | Sets the value or expression associated with this validation. |
| [setFormula2()](#setformula2) | Represents the value or expression associated with the data validation. |
| [setFormula2(formula, isR1C1, isLocal)](#setformula2-1) | Sets the value or expression associated with this validation. |
| [setIgnoreBlank()](#setignoreblank) | Indicates whether blank values are permitted by the range data validation. |
| [setInCellDropDown()](#setincelldropdown) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [setInputMessage()](#setinputmessage) | Represents the data validation input message. |
| [setInputTitle()](#setinputtitle) | Represents the title of the data-validation input dialog box. |
| [setOperator()](#setoperator) | Represents the operator for the data validation. The value of the property is OperatorType integer constant. |
| [setShowError()](#setshowerror) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [setShowInput()](#setshowinput) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data valid |
| [setType()](#settype) | Represents the data validation type. The value of the property is ValidationType integer constant. |
| [setValue1()](#setvalue1) | Represents the first value associated with the data validation. |
| [setValue2()](#setvalue2) | Represents the second value associated with the data validation. |

### addArea(cellArea) {#addarea}

Applies the validation to the area. It is equivalent to use addArea(com.aspose.cells.CellArea, boolean, boolean) with checking intersection and edge.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |

### addArea(cellArea, checkIntersection, checkEdge) {#addarea-1}

Applies the validation to the area. In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that the added area does not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if given area will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that the added area is not the top-left one, this parameter can be set as false for performance consideration. |

### addAreas(areas, checkIntersection, checkEdge) {#addareas}

Applies the validation to given areas. In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

| Parameter | Type | Description |
| --- | --- | --- |
| areas | Array ofCellArea | The areas. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |

### copy(source, copyOption) {#copy}

Copy validation.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Validation | The source validation. |
| copyOption | CopyOptions | The copy option. |

### getAlertStyle() {#getalertstyle}

Represents the validation alert style. The value of the property is ValidationAlertType integer constant.

### getAreas() {#getareas}

Gets all CellArea which contain the data validation settings.

### getErrorMessage() {#geterrormessage}

Represents the data validation error message.

### getErrorTitle() {#geterrortitle}

Represents the title of the data-validation error dialog box.

### getFormula1() {#getformula1}

Represents the value or expression associated with the data validation.

### getFormula1(isR1C1, isLocal) {#getformula1-1}

Gets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The value or expression associated with this validation.

### getFormula1(isR1C1, isLocal, row, column) {#getformula1-2}

Gets the value or expression associated with this validation for specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The value or expression associated with this validation.

### getFormula2() {#getformula2}

Represents the value or expression associated with the data validation.

### getFormula2(isR1C1, isLocal) {#getformula2-1}

Gets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The value or expression associated with this validation.

### getFormula2(isR1C1, isLocal, row, column) {#getformula2-2}

Gets the value or expression associated with this validation for specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The value or expression associated with this validation.

### getIgnoreBlank() {#getignoreblank}

Indicates whether blank values are permitted by the range data validation.

### getInCellDropDown() {#getincelldropdown}

Indicates whether data validation displays a drop-down list that contains acceptable values.

### getInputMessage() {#getinputmessage}

Represents the data validation input message.

### getInputTitle() {#getinputtitle}

Represents the title of the data-validation input dialog box.

### getListValue(row, column) {#getlistvalue}

Get the value for list of the validation for the specified cell. Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** Object — `Object` The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a ReferredArea object; Otherwise the returned value may be null, object[], or simple object.

### getOperator() {#getoperator}

Represents the operator for the data validation. The value of the property is OperatorType integer constant.

### getShowError() {#getshowerror}

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

### getShowInput() {#getshowinput}

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

### getType() {#gettype}

Represents the data validation type. The value of the property is ValidationType integer constant.

### getValue(row, column, isValue1) {#getvalue}

Get the value of validation on the specific cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |
| isValue1 | boolean | Indicates whether getting the first value. |

**Returns:** Object — `Object`

### getValue1() {#getvalue1}

Represents the first value associated with the data validation.

### getValue2() {#getvalue2}

Represents the second value associated with the data validation.

### removeACell(row, column) {#removeacell}

Remove the validation settings in the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

### removeArea(cellArea) {#removearea}

Remove the validation settings in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | the areas where this validation settings should be removed. |

### removeAreas(areas) {#removeareas}

Removes this validation from given areas.

| Parameter | Type | Description |
| --- | --- | --- |
| areas | Array ofCellArea | the areas where this validation settings should be removed. |

### setAlertStyle() {#setalertstyle}

Represents the validation alert style. The value of the property is ValidationAlertType integer constant.

### setErrorMessage() {#seterrormessage}

Represents the data validation error message.

### setErrorTitle() {#seterrortitle}

Represents the title of the data-validation error dialog box.

### setFormula1() {#setformula1}

Represents the value or expression associated with the data validation.

### setFormula1(formula, isR1C1, isLocal) {#setformula1-1}

Sets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2() {#setformula2}

Represents the value or expression associated with the data validation.

### setFormula2(formula, isR1C1, isLocal) {#setformula2-1}

Sets the value or expression associated with this validation.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setIgnoreBlank() {#setignoreblank}

Indicates whether blank values are permitted by the range data validation.

### setInCellDropDown() {#setincelldropdown}

Indicates whether data validation displays a drop-down list that contains acceptable values.

### setInputMessage() {#setinputmessage}

Represents the data validation input message.

### setInputTitle() {#setinputtitle}

Represents the title of the data-validation input dialog box.

### setOperator() {#setoperator}

Represents the operator for the data validation. The value of the property is OperatorType integer constant.

### setShowError() {#setshowerror}

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

### setShowInput() {#setshowinput}

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

### setType() {#settype}

Represents the data validation type. The value of the property is ValidationType integer constant.

### setValue1() {#setvalue1}

Represents the first value associated with the data validation.

### setValue2() {#setvalue2}

Represents the second value associated with the data validation.
