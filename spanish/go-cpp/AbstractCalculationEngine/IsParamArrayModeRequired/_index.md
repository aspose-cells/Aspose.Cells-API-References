---
title: "IsParamArrayModeRequired Método"
linktitle: "IsParamArrayModeRequired"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "IsParamArrayModeRequired método. Encapsula la función que representa isparamarraymoderequired en Go."
type: docs
weight: 200
url: /es/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false.If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating customfunctions and user has not updated the definition for them(by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)),this property needs to be set as true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Observaciones


## Ver también

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
