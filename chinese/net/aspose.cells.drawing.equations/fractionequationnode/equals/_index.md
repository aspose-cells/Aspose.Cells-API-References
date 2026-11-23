---
title: "FractionEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FractionEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

确定当前方程节点是否等于指定节点

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 指定的节点 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // 由于 FractionEquationNode 没有无参数构造函数，
                // 我们将使用可能来自 API 其他位置的对象来演示 Equals
                // 出于演示目的，我们假设有两个实例进行比较
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // 使用 Equals 比较这些对象
                bool areEqual = node1.Equals(node2);

                // 显示比较结果
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // 与 null 比较
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // 与自身比较
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // 辅助方法，用于模拟获取 FractionEquationNode 实例
        // (在实际使用中，这些会来自 API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // 这只是一个占位符——实际上你会从 API 获取这些
            // 例如：worksheet.Equations.AddFractionEquationNode() 或类似方法
            return null; // Actual implementation would depend on API
        }
    }
}
```

### 另请参见

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


