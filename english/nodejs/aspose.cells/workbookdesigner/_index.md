---
title: "WorkbookDesigner"
linktitle: "WorkbookDesigner"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a designer spreadsheet."
type: docs
weight: 4680
url: /nodejs/aspose.cells/workbookdesigner/
---

## WorkbookDesigner class

Encapsulates the object that represents a designer spreadsheet.

```js
new WorkbookDesigner()
```

Initializes a new instance of the WorkbookDesigner class.

## Methods

| Name | Description |
| --- | --- |
| [clearDataSource()](#cleardatasource) | Clears all data sources. |
| [constructor_overload$1(workbook)](#constructor-overload1) | Initializes a new instance of the WorkbookDesigner class. |
| [containsVariables()](#containsvariables) |  |
| [getCalculateFormula()](#getcalculateformula) | Indicates whether formulas should be calculated. |
| [getLineByLine()](#getlinebyline) | Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must  |
| [getRepeatFormulasWithSubtotal()](#getrepeatformulaswithsubtotal) | Indicates whether repeating formulas with subtotal row. |
| [getSmartMarkers()](#getsmartmarkers) | Returns a collection of smart markers in a spreadsheet. A string array is created on every call. The array is sorted and |
| [getSortDataSource()](#getsortdatasource) |  |
| [getUpdateEmptyStringAsNull()](#getupdateemptystringasnull) | If TRUE, Null will be inserted if the value is ""; |
| [getUpdateReference()](#getupdatereference) | Indicates if references in other worksheets will be updated. |
| [getVariablesWorksheetName()](#getvariablesworksheetname) |  |
| [getWorkbook()](#getworkbook) | Gets and sets the Workbook object. |
| [process()](#process) |  |
| [process()](#process-1) | Processes the smart markers and populates the data source values. |
| [process(isPreserved)](#process-2) | Processes the smart markers and populates the data source values. |
| [process(sheetIndex, isPreserved)](#process-3) | Processes the smart markers and populates the data source values. This method works on worksheet level. |
| [setCalculateFormula()](#setcalculateformula) | Indicates whether formulas should be calculated. |
| [setContainsVariables()](#setcontainsvariables) |  |
| [setDataSource(variable, data)](#setdatasource) | Sets data binding to a variable. |
| [setJsonDataSource(variable, data)](#setjsondatasource) |  |
| [setLineByLine()](#setlinebyline) | Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must  |
| [setRepeatFormulasWithSubtotal()](#setrepeatformulaswithsubtotal) | Indicates whether repeating formulas with subtotal row. |
| [setSortDataSource()](#setsortdatasource) |  |
| [setUpdateEmptyStringAsNull()](#setupdateemptystringasnull) | If TRUE, Null will be inserted if the value is ""; |
| [setUpdateReference()](#setupdatereference) | Indicates if references in other worksheets will be updated. |
| [setVariablesWorksheetName()](#setvariablesworksheetname) |  |
| [setWorkbook()](#setworkbook) | Gets and sets the Workbook object. |

### clearDataSource() {#cleardatasource}

Clears all data sources.

### constructor_overload$1(workbook) {#constructor-overload1}

Initializes a new instance of the WorkbookDesigner class.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |

### containsVariables() {#containsvariables}

### getCalculateFormula() {#getcalculateformula}

Indicates whether formulas should be calculated.

### getLineByLine() {#getlinebyline}

Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".

### getRepeatFormulasWithSubtotal() {#getrepeatformulaswithsubtotal}

Indicates whether repeating formulas with subtotal row.

### getSmartMarkers() {#getsmartmarkers}

Returns a collection of smart markers in a spreadsheet. A string array is created on every call. The array is sorted and duplicated values are removed.@return {String[]} A collection of smart markers

### getSortDataSource() {#getsortdatasource}

### getUpdateEmptyStringAsNull() {#getupdateemptystringasnull}

If TRUE, Null will be inserted if the value is "";

### getUpdateReference() {#getupdatereference}

Indicates if references in other worksheets will be updated.

### getVariablesWorksheetName() {#getvariablesworksheetname}

### getWorkbook() {#getworkbook}

Gets and sets the Workbook object.

### process() {#process}

### process() {#process-1}

Processes the smart markers and populates the data source values.

### process(isPreserved) {#process-2}

Processes the smart markers and populates the data source values.

| Parameter | Type | Description |
| --- | --- | --- |
| isPreserved | boolean | True if the unrecognized smart marker is preserved. |

### process(sheetIndex, isPreserved) {#process-3}

Processes the smart markers and populates the data source values. This method works on worksheet level.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | Worksheet index. |
| isPreserved | boolean | True if the unrecognized smart marker is preserved. |

### setCalculateFormula() {#setcalculateformula}

Indicates whether formulas should be calculated.

### setContainsVariables() {#setcontainsvariables}

### setDataSource(variable, data) {#setdatasource}

Sets data binding to a variable.

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| data | Object | Source data. |

### setJsonDataSource(variable, data) {#setjsondatasource}

| Parameter | Description |
| --- | --- |
| variable |  |
| data |  |

### setLineByLine() {#setlinebyline}

Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".

### setRepeatFormulasWithSubtotal() {#setrepeatformulaswithsubtotal}

Indicates whether repeating formulas with subtotal row.

### setSortDataSource() {#setsortdatasource}

### setUpdateEmptyStringAsNull() {#setupdateemptystringasnull}

If TRUE, Null will be inserted if the value is "";

### setUpdateReference() {#setupdatereference}

Indicates if references in other worksheets will be updated.

### setVariablesWorksheetName() {#setvariablesworksheetname}

### setWorkbook() {#setworkbook}

Gets and sets the Workbook object.
