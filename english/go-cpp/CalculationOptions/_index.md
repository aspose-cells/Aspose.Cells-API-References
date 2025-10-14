---
title: CalculationOptions Class 
linktitle: CalculationOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'CalculationOptions class. Encapsulates the object that represents calculationoptions in Go.'
type: docs
weight: 200
url: /go-cpp/calculationoptions/
---

## CalculationOptions class

Represents options for calculation.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewCalculationOptions](./newcalculationoptions/) | Default constructor. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetIgnoreError](./getignoreerror/) | Indicates whether errors encountered while calculating formulas should be ignored.The error may be unsupported function, external links, etc.The default value is true. | 
|[SetIgnoreError](./setignoreerror/) | Indicates whether errors encountered while calculating formulas should be ignored.The error may be unsupported function, external links, etc.The default value is true. | 
|[GetRecursive](./getrecursive/) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells.The default value is true. | 
|[SetRecursive](./setrecursive/) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells.The default value is true. | 
|[GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Indicates whether user has explicitly specified the behavior ofrefreshing dynamic array formulas before calculating specified formulas. | 
|[GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Indicates whether dynamic array formulas should be refreshedbefore calculating formulas. | 
|[SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Indicates whether dynamic array formulas should be refreshedbefore calculating formulas. | 
|[GetCustomEngine](./getcustomengine/) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. | 
|[SetCustomEngine](./setcustomengine/) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. | 
|[GetCalcStackSize](./getcalcstacksize/) | The stack size for calculating cells recursively. Default value is 200. | 
|[SetCalcStackSize](./setcalcstacksize/) | The stack size for calculating cells recursively. Default value is 200. | 
|[GetPrecisionStrategy](./getprecisionstrategy/) | Specifies the strategy for processing precision of calculation. | 
|[SetPrecisionStrategy](./setprecisionstrategy/) | Specifies the strategy for processing precision of calculation. | 
|[GetLinkedDataSources](./getlinkeddatasources/) | Specifies the data sources for external links used in formulas. | 
|[SetLinkedDataSources](./setlinkeddatasources/) | Specifies the data sources for external links used in formulas. | 
|[GetCharacterEncoding](./getcharacterencoding/) | Specifies the encoding used for encoding/decoding characters when calculating formulas.For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment.With this property user can specify the proper encoding used for those function to get the expected result. | 
|[SetCharacterEncoding](./setcharacterencoding/) | Specifies the encoding used for encoding/decoding characters when calculating formulas.For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment.With this property user can specify the proper encoding used for those function to get the expected result. | 
