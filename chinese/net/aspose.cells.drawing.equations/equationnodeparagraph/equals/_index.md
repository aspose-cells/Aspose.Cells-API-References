---
title: "EquationNodeParagraph.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNodeParagraph 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

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

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建两个 EquationNodeParagraph 实例用于比较
            // 使用 CreateNode 方法正确实例化节点
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // 设置不同的对齐类型使它们不相等
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // 使用 paragraph2 作为参数调用 Equals 方法
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // 显示比较结果
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // 创建另一个段落，其对齐方式与 paragraph1 相同
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // 再次使用 paragraph3 调用 Equals
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // 还演示与 null 的比较
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // 保存工作簿（尽管工作表没有可见的更改）
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


