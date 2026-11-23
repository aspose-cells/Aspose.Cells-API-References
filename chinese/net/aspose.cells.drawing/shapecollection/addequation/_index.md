---
title: "ShapeCollection.AddEquation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapeCollection 方法。向工作表添加一个方程对象"
type: docs
url: /zh/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

向工作表添加一个公式对象。

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | Int32 | 顶部行索引。 |
| 顶部 | Int32 | 其顶部行的垂直偏移量，单位为像素。 |
| leftColumn | Int32 | 左列索引。 |
| 左 | Int32 | 水平偏移量相对于其左列，单位为像素。 |
| height | Int32 | 公式的高度，单位为像素。 |
| 宽度 | Int32 | 公式的宽度，单位为像素。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fraction.FractionType = EquationFractionType.Skewed;

            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numText.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denText.Text = "B";

            workbook.Save("ShapeEquationDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


