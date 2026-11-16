---
title: "AbstractCalculationEngine 类"
linktitle: "AbstractCalculationEngine"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AbstractCalculationEngine 类。封装在 Go 中表示 abstractcalculationengine 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

表示用户的自定义计算引擎，以扩展 Aspose.Cells 的默认计算引擎。

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | 跳过对引用当前正在评估的函数的整个公式的计算。 |
| [IsParamLiteralRequired](./isparamliteralrequired/) | 指示此引擎在进行计算时是否需要参数的文字文本。默认值为 false。 |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | 指示此引擎是否需要在数组模式下计算参数。默认值为 false。如果在计算自定义函数时需要 CalculationData.GetParamValueInArrayMode(int, int, int) 且用户尚未通过 Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) 更新其定义，则此属性需要设为 true。 |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | 是否应检查并处理由内置引擎支持的内置函数。默认值为 false。 |
| [ForceRecalculate](./forcerecalculate/) | 是否在计算共享公式时强制始终重新计算给定函数。 |
