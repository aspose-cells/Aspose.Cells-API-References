---
title: "类 RadicalEquationNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.RadicalEquationNode 类。此类指定由可选次数 degEquationNodeType.Degree 和底数组成的根式方程"
type: docs
url: /zh/net/aspose.cells.drawing.equations/radicalequationnode/
---
## RadicalEquationNode class

此类指定根式方程，由可选的次数 deg(EquationNodeType.Degree) 和基数组成。

```csharp
public class RadicalEquationNode : EquationNode
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | 获取当前节点的方程类型（继承自 [`EquationNode`](../equationnode/)。） |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | 返回此对象的字体。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [IsDegHide](../../aspose.cells.drawing.equations/radicalequationnode/isdeghide/) { get; set; } | 是否隐藏根式的次数。 |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | 获取字符的长度。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | 指定当前节点的父节点（继承自 [`EquationNode`](../equationnode/)。） |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | 获取字符的起始索引。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | 返回文本选项。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | 表示节点的类型。（继承自 [`EquationNode`](../equationnode/)。） |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | 在当前节点的子节点列表末尾插入指定节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | 在当前节点的子节点列表末尾插入指定类型的节点。（继承自 [`EquationNode`](../equationnode/)。） |
| override [Equals](../../aspose.cells.drawing.equations/radicalequationnode/equals/)(object) | 确定当前方程节点是否等于指定节点 |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | 返回当前节点子节点中指定索引处的节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | 在当前节点之后插入指定节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | 在当前节点之前插入指定节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | 在当前节点的子节点列表中指定索引位置插入指定类型的节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | 从父节点中移除自身。（继承自 [`EquationNode`](../equationnode/)。） |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | 移除当前节点的所有子节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | 从当前节点的子节点中移除指定节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | 从当前节点的子节点中移除指定索引处的节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | 设置预设的 WordArt 样式。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | 将此 equtation 转换为 LaTeX 表达式。（继承自 [`EquationNode`](../equationnode/)。） |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | 将此 equtation 转换为 MathML 表达式。（继承自 [`EquationNode`](../equationnode/)。） |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassRadicalEquationNodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 在第一个工作表中添加带公式的文本框
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 获取方程节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // 添加根式方程节点
            RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            radicalNode.IsDegHide = true;

            // 添加次数（隐藏）和底数组件
            EquationNode degreeNode = radicalNode.AddChild(EquationNodeType.Degree);
            TextRunEquationNode degreeText = (TextRunEquationNode)degreeNode.AddChild(EquationNodeType.Text);
            degreeText.Text = "3";

            EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x + 1";

            // 保存工作簿
            workbook.Save("RadicalEquationDemo.xlsx");

            // 加载已保存的工作簿进行验证
            Workbook loadedWorkbook = new Workbook("RadicalEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            RadicalEquationNode loadedRadicalNode = (RadicalEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("Radical equation created successfully:");
            Console.WriteLine($"- IsDegHide: {loadedRadicalNode.IsDegHide}");
            Console.WriteLine($"- Base text: {((TextRunEquationNode)loadedRadicalNode.GetChild(1).GetChild(0)).Text}");
        }
    }
}
```

### 另请参见

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


