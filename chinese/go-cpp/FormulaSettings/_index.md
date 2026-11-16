---
title: "FormulaSettings 类"
linktitle: "FormulaSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FormulaSettings 类。封装在 Go 中表示 formulasettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/formulasettings/
---

## FormulaSettings class

公式和计算的设置。

```go

type FormulaSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCalculateOnOpen](./getcalculateonopen/) | 指示在打开工作簿时应用程序是否需要执行完整计算。 |
| [SetCalculateOnOpen](./setcalculateonopen/) | 指示在打开工作簿时应用程序是否需要执行完整计算。 |
| [GetCalculateOnSave](./getcalculateonsave/) | 指示在手动计算模式下，保存文档前是否重新计算工作簿。 |
| [SetCalculateOnSave](./setcalculateonsave/) | 指示在手动计算模式下，保存文档前是否重新计算工作簿。 |
| [GetForceFullCalculation](./getforcefullcalculation/) | 指示在触发计算时是否每次都计算所有公式。 |
| [SetForceFullCalculation](./setforcefullcalculation/) | 指示在触发计算时是否每次都计算所有公式。 |
| [GetCalculationMode](./getcalculationmode/) | 获取或设置在 MS Excel 中工作簿计算的模式。 |
| [SetCalculationMode](./setcalculationmode/) | 获取或设置在 MS Excel 中工作簿计算的模式。 |
| [GetCalculationId](./getcalculationid/) | 指定用于计算工作簿中数值的计算引擎版本。 |
| [SetCalculationId](./setcalculationid/) | 指定用于计算工作簿中数值的计算引擎版本。 |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | 指示是否启用迭代计算以解决循环引用。 |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | 指示是否启用迭代计算以解决循环引用。 |
| [GetMaxIteration](./getmaxiteration/) | 解决循环引用的最大迭代次数。 |
| [SetMaxIteration](./setmaxiteration/) | 解决循环引用的最大迭代次数。 |
| [GetMaxChange](./getmaxchange/) | 解决循环引用的最大变化量。 |
| [SetMaxChange](./setmaxchange/) | 解决循环引用的最大变化量。 |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | 指示在计算公式时是否将计算结果的精度设置为显示的方式。 |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | 指示在计算公式时是否将计算结果的精度设置为显示的方式。 |
| [GetEnableCalculationChain](./getenablecalculationchain/) | 指示是否为公式启用计算链。默认值为 false。 |
| [SetEnableCalculationChain](./setenablecalculationchain/) | 指示是否为公式启用计算链。默认值为 false。 |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。 |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。 |
