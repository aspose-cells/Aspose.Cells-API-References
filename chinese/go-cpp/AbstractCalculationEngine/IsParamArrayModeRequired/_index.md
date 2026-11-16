---
title: "IsParamArrayModeRequired 方法"
linktitle: "IsParamArrayModeRequired"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "IsParamArrayModeRequired 方法。封装了在 Go 中表示 isparamarraymoderequired 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

指示此引擎是否需要在数组模式下计算参数。默认值为 false。如果在计算自定义函数时需要 CalculationData.GetParamValueInArrayMode(int, int, int) 且用户尚未通过 Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) 更新其定义，则此属性需要设为 true。

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## 备注


## 另请参阅

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
