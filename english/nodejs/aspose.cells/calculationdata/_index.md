---
title: "CalculationData"
linktitle: "CalculationData"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the required data when calculating one function, such as function name, parameters, ...etc."
type: docs
weight: 320
url: /nodejs/aspose.cells/calculationdata/
---

## CalculationData class

Represents the required data when calculating one function, such as function name, parameters, ...etc. All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

## Methods

| Name | Description |
| --- | --- |
| [getCalculatedValue()](./getcalculatedvalue/) | Gets or sets the calculated value for this function. User should set this property in his custom calculation engine for  |
| [getCell()](./getcell/) | Gets the Cell object where the function is in. When calculating a formula without setting it to a cell, such as by Works |
| [getCellColumn()](./getcellcolumn/) | Gets the column index of the cell where the function is in. |
| [getCellRow()](./getcellrow/) | Gets the row index of the cell where the function is in. |
| [getFunctionName()](./getfunctionname/) | Gets the function name to be calculated. |
| [getParamCount()](./getparamcount/) | Gets the count of parameters |
| [getParamText(index)](./getparamtext/) | Gets the literal text of the parameter at given index. |
| [getParamValue(index)](./getparamvalue/) | Gets the represented value object of the parameter at given index. For one parameter: If it is plain value, then returns |
| [getParamValueInArrayMode(index, maxRowCount, maxColumnCount)](./getparamvalueinarraymode/) | Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculat |
| [getWorkbook()](./getworkbook/) | Gets the Workbook object where the function is in. |
| [getWorksheet()](./getworksheet/) | Gets the Worksheet object where the function is in. |
| [setCalculatedValue()](./setcalculatedvalue/) | Gets or sets the calculated value for this function. User should set this property in his custom calculation engine for  |
