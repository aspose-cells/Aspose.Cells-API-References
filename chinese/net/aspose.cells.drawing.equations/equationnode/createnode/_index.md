---
title: "EquationNode.CreateNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 方法。创建指定类型的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

创建指定类型的节点。

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| equationType | EquationNodeType | Equation 节点的类型 |
| 工作簿 | Workbook | 与方程关联的工作簿对象 |
| 父节点 | EquationNode | 此节点所在的父节点 |

### 返回值

如果指定的类型存在，则返回相应的节点；如果该类型不存在，则返回未知类型的节点。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建方程形状
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // 创建父节点（分数）
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // 创建分子和分母节点
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // 将创建的分数添加到主方程中
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // 在单元格中显示方程
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


