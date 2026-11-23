---
title: "EquationNode.InsertAfter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 方法。在当前节点后插入指定节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

在当前节点之后插入指定节点。

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | EquationNodeType | Equation 节点的类型 |

### 返回值

如果指定的类型存在，则返回相应的节点；如果该类型不存在，则返回未知类型的节点。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 在单元格 A1 中创建公式形状
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // 添加初始文本节点
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // 在现有节点后插入新的文本节点
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // 显示公式结构
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // 将方程保存到单元格以进行可视化检查
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


