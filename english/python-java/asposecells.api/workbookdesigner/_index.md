---
title: "WorkbookDesigner Class"
linktitle: "WorkbookDesigner"
articleTitle: "WorkbookDesigner"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents a designer spreadsheet."
type: docs
weight: 7550
url: /python-java/asposecells.api/workbookdesigner/
---

## WorkbookDesigner class

Encapsulates the object that represents a designer spreadsheet.

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookDesigner](#constructor) | Initializes a new instance of the WorkbookDesigner class. |
| [WorkbookDesigner](#constructor) | Initializes a new instance of the WorkbookDesigner class. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Workbook](#workbook) | Workbook | Gets and sets the Workbook object. |
| [RepeatFormulasWithSubtotal](#repeatformulaswithsubtotal) | boolean | Indicates whether repeating formulas with subtotal row. |
| [UpdateEmptyStringAsNull](#updateemptystringasnull) | boolean | If TRUE, Null will be inserted if the value is ""; |
| [UpdateReference](#updatereference) | boolean | Indicates if references in other worksheets will be updated. |
| [CalculateFormula](#calculateformula) | boolean | Indicates whether formulas should be calculated. |
| [LineByLine](#linebyline) | boolean | Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must  |
| [ContainsVariables](#containsvariables) | boolean |  |
| [VariablesWorksheetName](#variablesworksheetname) | String |  |
| [SortDataSource](#sortdatasource) | boolean |  |

## Methods

| Name | Description |
| --- | --- |
| [clearDataSource](#cleardatasource) | Clears all data sources. |
| [setJsonDataSource](#setjsondatasource) |  |
| [setDataSource](#setdatasource) | Sets data binding to a variable. |
| [process](#process) |  |
| [getSmartMarkers](#getsmartmarkers) | Returns a collection of smart markers in a spreadsheet.

A string array is created on every call. The array is sorted an |

### WorkbookDesigner() (1 of 2) {#constructor}

Initializes a new instance of the WorkbookDesigner class.

---

### WorkbookDesigner(workbook) (2 of 2) {#constructor-1}

Initializes a new instance of the WorkbookDesigner class.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |

### WorkbookDesigner.Workbook property {#workbook}

Gets and sets the Workbook object.

**Type:** Workbook

### WorkbookDesigner.RepeatFormulasWithSubtotal property {#repeatformulaswithsubtotal}

Indicates whether repeating formulas with subtotal row.

**Type:** boolean

### WorkbookDesigner.UpdateEmptyStringAsNull property {#updateemptystringasnull}

If TRUE, Null will be inserted if the value is "";

**Type:** boolean

### WorkbookDesigner.UpdateReference property {#updatereference}

Indicates if references in other worksheets will be updated.

**Type:** boolean

### WorkbookDesigner.CalculateFormula property {#calculateformula}

Indicates whether formulas should be calculated.

**Type:** boolean

### WorkbookDesigner.LineByLine property {#linebyline}

Indicates whether processing the smart marker line by line. The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".

**Type:** boolean

### WorkbookDesigner.ContainsVariables property {#containsvariables}

**Type:** boolean

### WorkbookDesigner.VariablesWorksheetName property {#variablesworksheetname}

**Type:** String

### WorkbookDesigner.SortDataSource property {#sortdatasource}

**Type:** boolean

### clearDataSource() {#cleardatasource}

Clears all data sources.

### setJsonDataSource(name, json) {#setjsondatasource}

| Parameter | Type | Description |
| --- | --- | --- |
| variable |  |  |
| data |  |  |

### setDataSource(variable, data) {#setdatasource}

Sets data binding to a variable.

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| data | Object | Source data. |

### process(range, isPreserved) (1 of 4) {#process}

---

### process() (2 of 4) {#process-1}

Processes the smart markers and populates the data source values.

---

### process(isPreserved) (3 of 4) {#process-2}

Processes the smart markers and populates the data source values.

| Parameter | Type | Description |
| --- | --- | --- |
| isPreserved | boolean | True if the unrecognized smart marker is preserved. |

---

### process(sheetIndex, isPreserved) (4 of 4) {#process-3}

Processes the smart markers and populates the data source values.

This method works on worksheet level.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Worksheet index. |
| isPreserved | boolean | True if the unrecognized smart marker is preserved. |

### getSmartMarkers() {#getsmartmarkers}

Returns a collection of smart markers in a spreadsheet.

A string array is created on every call. The array is sorted and duplicated values are removed.

**Returns:** A collection of smart markers
