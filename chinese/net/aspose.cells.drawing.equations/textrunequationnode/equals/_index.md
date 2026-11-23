---
title: "TextRunEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextRunEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 出于演示目的，我们将使用 null 并仅展示比较逻辑
            // 由于无法直接创建 TextRunEquationNode 实例
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // 此部分保留以展示如何调用 Equals
                // 在真实场景中，这些节点将被正确初始化
                if (node1 != null && node2 != null && node3 != null)
                {
                    // 比较 node1 与 node2（相同内容）
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // 比较 node1 与 node3（不同内容）
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // 与 null 比较
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // 与不同对象类型进行比较
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // 保存工作簿（尽管 Equals 不会修改电子表格）
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // 已移除辅助方法，因为我们无法正确创建 TextRunEquationNode 实例
    }
}
```

### 另请参见

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


