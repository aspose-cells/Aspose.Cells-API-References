---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MatrixEquationNode 属性。此属性指定矩阵上的隐藏占位符属性。当此属性开启时，占位符不会出现在矩阵中。默认情况下，占位符会出现，使得可以插入文本的位置可见"
type: docs
url: /zh/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

此属性指定矩阵的隐藏占位符属性。启用此属性时，占位符不会出现在矩阵中。默认情况下，占位符会出现，以便显示可插入文本的位置。

```csharp
public bool IsHidePlaceholder { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加公式形状
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 获取数学节点并添加矩阵
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // 设置矩阵属性
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // 添加对角线为 1 的 2x2 矩阵
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // 保存并验证
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### 另请参见

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


