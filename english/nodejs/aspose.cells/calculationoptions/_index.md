---
title: "CalculationOptions"
linktitle: "CalculationOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents options for calculation."
type: docs
weight: 330
url: /nodejs/aspose.cells/calculationoptions/
---

## CalculationOptions class

Represents options for calculation.

```js
new CalculationOptions()
```

## Methods

| Name | Description |
| --- | --- |
| [getCalcStackSize()](#getcalcstacksize) | The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be  |
| [getCalculationMonitor()](#getcalculationmonitor) | The monitor for user to track the progress of formula calculation. |
| [getCharacterEncoding()](#getcharacterencoding) | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE |
| [getIgnoreError()](#getignoreerror) | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function |
| [getLinkedDataSources()](#getlinkeddatasources) | Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Wo |
| [getPrecisionStrategy()](#getprecisionstrategy) | Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrateg |
| [getRecursive()](#getrecursive) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The |
| [getRefreshDynamicArrayFormula()](#getrefreshdynamicarrayformula) |  |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getuserspecifiedrefreshdynamicarrayformula) |  |
| [setCalcStackSize()](#setcalcstacksize) | The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be  |
| [setCalculationMonitor()](#setcalculationmonitor) | The monitor for user to track the progress of formula calculation. |
| [setCharacterEncoding()](#setcharacterencoding) | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE |
| [setIgnoreError()](#setignoreerror) | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function |
| [setLinkedDataSources()](#setlinkeddatasources) | Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Wo |
| [setPrecisionStrategy()](#setprecisionstrategy) | Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrateg |
| [setRecursive()](#setrecursive) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The |
| [setRefreshDynamicArrayFormula()](#setrefreshdynamicarrayformula) |  |

### getCalcStackSize() {#getcalcstacksize}

The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### getCalculationMonitor() {#getcalculationmonitor}

The monitor for user to track the progress of formula calculation.

### getCharacterEncoding() {#getcharacterencoding}

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

### getIgnoreError() {#getignoreerror}

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

### getLinkedDataSources() {#getlinkeddatasources}

Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]).

### getPrecisionStrategy() {#getprecisionstrategy}

Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrategy integer constant.

### getRecursive() {#getrecursive}

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

### getRefreshDynamicArrayFormula() {#getrefreshdynamicarrayformula}

### getUserSpecifiedRefreshDynamicArrayFormula() {#getuserspecifiedrefreshdynamicarrayformula}

### setCalcStackSize() {#setcalcstacksize}

The stack size for calculating cells recursively. Default value is 200. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### setCalculationMonitor() {#setcalculationmonitor}

The monitor for user to track the progress of formula calculation.

### setCharacterEncoding() {#setcharacterencoding}

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

### setIgnoreError() {#setignoreerror}

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

### setLinkedDataSources() {#setlinkeddatasources}

Specifies the data sources for external links used in formulas. Like Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by Workbook.updateLinkedDataSource(com.aspose.cells.Workbook[]).

### setPrecisionStrategy() {#setprecisionstrategy}

Specifies the strategy for processing precision of calculation. The value of the property is CalculationPrecisionStrategy integer constant.

### setRecursive() {#setrecursive}

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

### setRefreshDynamicArrayFormula() {#setrefreshdynamicarrayformula}
