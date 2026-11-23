---
title: "UnknowEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "UnknowEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建两个未知方程节点用于比较
            // 由于 UnknowEquationNode 没有无参构造函数，
            // 我们需要以不同方式创建它们。演示目的下，我们将使用
            // 实际构造函数（如果可用），或通过其他方式创建它们。
            // 由于我们不知道构造函数参数，这是一种占位修复。
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // 使用特定参数类型 (Object) 调用 Equals 方法
                bool areEqual = node1.Equals(objToCompare);

                // 显示结果
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // 将结果添加到工作表中
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // 帮助方法用于创建 UnknowEquationNode 实例
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // 在真实实现中，这将使用适当的构造函数
            // 由于我们不知道构造函数参数，我们将返回 null
            // 并在演示中处理 null 情况（尽管这只是一个占位符）
            return null;
        }
    }
}
```

### 另请参见

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


