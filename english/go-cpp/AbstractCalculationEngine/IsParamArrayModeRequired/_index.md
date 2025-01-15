---
title: IsParamArrayModeRequired Method 
linktitle: IsParamArrayModeRequired
second_title: Aspose.Cells for Go via C++ API Reference
description: 'IsParamArrayModeRequired method. Encapsulates the function that represents isparamarraymoderequired in Go.'
type: docs
weight: 200
url: /go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false.If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating customfunctions and user has not updated the definition for them(by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)),this property needs to be set as true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Remarks


## See Also

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
