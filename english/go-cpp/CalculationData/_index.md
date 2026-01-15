---
title: CalculationData Class 
linktitle: CalculationData
second_title: Aspose.Cells for Go via C++ API Reference
description: 'CalculationData class. Encapsulates the object that represents calculationdata in Go.'
type: docs
weight: 200
url: /go-cpp/calculationdata/
---

## CalculationData class

Represents the required data when calculating one function, such as function name, parameters, ...etc.

```go

type CalculationData struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetCalculatedValue](./getcalculatedvalue/) | Gets or sets the calculated value for this function. | 
|[SetCalculatedValue](./setcalculatedvalue/) | Gets or sets the calculated value for this function. | 
|[GetWorkbook](./getworkbook/) | Gets the Workbook object where the function is. | 
|[GetWorksheet](./getworksheet/) | Gets the Worksheet object where the function is. | 
|[GetCellRow](./getcellrow/) | Gets the row index of the cell where the function is. | 
|[GetCellColumn](./getcellcolumn/) | Gets the column index of the cell where the function is. | 
|[GetCell](./getcell/) | Gets the Cell object where the function is. | 
|[GetFunctionName](./getfunctionname/) | Gets the function name to be calculated. | 
|[GetParamCount](./getparamcount/) | Gets the count of parameters | 
|[GetParamValue](./getparamvalue/) | Gets the represented value object of the parameter at a given index. | 
|[GetParamValueInArrayMode](./getparamvalueinarraymode/) | Gets the value(s) of the parameter at a given index.If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. | 
|[GetParamText](./getparamtext/) | Gets the literal text of the parameter at the given index. | 
