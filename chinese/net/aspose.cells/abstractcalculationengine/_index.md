---
title: AbstractCalculationEngine
second_title: Aspose.Cells for .NET API 参考
description: 代表用户自定义计算引擎扩展Aspose.Cells的默认计算引擎
type: docs
weight: 20
url: /zh/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

代表用户自定义计算引擎，扩展Aspose.Cells的默认计算引擎。

```csharp
public abstract class AbstractCalculationEngine
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired) { get; } | 表示该引擎在计算时是否需要参数的文字文本。默认值为假。 |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions) { get; } | 内置引擎已经支持的内置函数是否应该由本实现检查处理。 默认为false。 如果用户需要更改某些内置函数的计算逻辑，该属性应该是设置为真。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate)(CalculationData) | 用给定的数据计算一个函数。 |

### 评论

用户不应在此实现中直接修改 Workbook 的任何部分（自定义函数的计算结果除外，可以通过 CalculationData.CalculatedValue 属性设置）。 否则可能会导致意外结果或异常。 如果用户需要更改某些自定义函数的实现中计算结果以外的其他数据， 例如，更改单元格的公式、样式等，用户应在此实现中收集这些数据并将其更改为公式计算范围之外。

### 例子

```csharp
[C#]
public class MyEngine : AbstractCalculationEngine
{
    public override void Calculate(CalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //这里计算MYFUNC
            int count = data.ParamCount;
            object res = null;
            for (int i = 0; i < count; i++)
            {
                object pv = data.GetParamValue(i);
                if (pv is ReferredArea)
                {
                    ReferredArea ra = (ReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                //这里处理参数
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
