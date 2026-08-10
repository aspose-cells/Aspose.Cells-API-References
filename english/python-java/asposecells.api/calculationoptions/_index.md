---
title: "CalculationOptions Class"
linktitle: "CalculationOptions"
articleTitle: "CalculationOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents options for calculation."
type: docs
weight: 500
url: /python-java/asposecells.api/calculationoptions/
---

## CalculationOptions class

Represents options for calculation.

## Constructors

| Name | Description |
| --- | --- |
| [CalculationOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IgnoreError](#ignoreerror) | boolean | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function |
| [Recursive](#recursive) | boolean | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The |
| [UserSpecifiedRefreshDynamicArrayFormula](#userspecifiedrefreshdynamicarrayformula) | boolean |  |
| [RefreshDynamicArrayFormula](#refreshdynamicarrayformula) | boolean |  |
| [CalculationMonitor](#calculationmonitor) | AbstractCalculationMonitor | The monitor for user to track the progress of formula calculation. |
| [CalcStackSize](#calcstacksize) | int | The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be  |
| [PrecisionStrategy](#precisionstrategy) | int | Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrateg |
| [LinkedDataSources](#linkeddatasources) | Workbook[] | Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Wo |
| [CharacterEncoding](#characterencoding) | Encoding | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE |

### CalculationOptions() {#constructor}

### CalculationOptions.IgnoreError property {#ignoreerror}

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

**Type:** boolean

### CalculationOptions.Recursive property {#recursive}

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

**Type:** boolean

### CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property {#userspecifiedrefreshdynamicarrayformula}

**Type:** boolean

### CalculationOptions.RefreshDynamicArrayFormula property {#refreshdynamicarrayformula}

**Type:** boolean

### CalculationOptions.CalculationMonitor property {#calculationmonitor}

The monitor for user to track the progress of formula calculation.

**Type:** AbstractCalculationMonitor

### CalculationOptions.CalcStackSize property {#calcstacksize}

The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

**Type:** int

### CalculationOptions.PrecisionStrategy property {#precisionstrategy}

Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrategy integer constant.

**Type:** int

### CalculationOptions.LinkedDataSources property {#linkeddatasources}

Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]) , here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]) .

**Type:** Workbook[]

### CalculationOptions.CharacterEncoding property {#characterencoding}

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

**Type:** Encoding
