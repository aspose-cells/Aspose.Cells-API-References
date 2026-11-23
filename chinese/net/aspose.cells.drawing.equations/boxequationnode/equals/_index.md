---
title: "BoxEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "BoxEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建两个 BoxEquationNode 对象以进行比较
            // 由于 BoxEquationNode 没有无参数构造函数，
            // 我们需要以不同方式创建它们。假设我们可以从某处获取它们，
            // 或者使用一些默认参数创建它们。
            // 出于演示目的，我们只会声明它们并赋值为 null（虽然在实际代码中需要进行适当的初始化）
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // 调用 Equals 方法并使用特定的参数类型（Object）
                    bool areEqual = node1.Equals(objToCompare);

                    // 显示结果
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // 将结果添加到工作表中
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // 保存结果
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


