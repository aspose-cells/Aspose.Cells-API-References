---
title: "类 NaryEquationNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode 类。此类指定由 nary 运算符、基数或操作数以及可选的上限和下限组成的 nary 运算符方程。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

此类指定 n 元运算符方程，由 n 元运算符、基数（或操作数）以及可选的上界和下界组成。

```csharp
public class NaryEquationNode : EquationNode
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | 获取当前节点的方程类型（继承自 [`EquationNode`](../equationnode/)。） |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | 返回此对象的字体。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | 是否显示下限 |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | 是否显示上限 |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | 获取字符的长度。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | 此属性指定 n-ary 运算符中极限的位置。极限可以居中于 n-ary 运算符的上方和下方，或仅位于运算符的右侧。 |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | an n-ary operator.e.g "∑". It is strongly recommended to use attribute NaryOperatorType to set n-ary operator. Use this property setting if you cannot find the character you need in a known type. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | an n-ary operator.e.g "∑" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | 指定当前节点的父节点（继承自 [`EquationNode`](../equationnode/)。） |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | 获取字符的起始索引。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | 返回文本选项。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | 表示节点的类型。（继承自 [`EquationNode`](../equationnode/)。） |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | 在当前节点的子节点列表末尾插入指定节点。（继承自 [`EquationNode`](../equationnode/)。） |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | 在当前节点的子节点列表末尾插入指定类型的节点。（继承自 [`EquationNode`](../equationnode/)。） |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | 确定当前方程节点是否等于指定节点 |
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
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an equation shape
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 获取方程节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Create a nary equation node
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Set nary properties
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Add base component
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // 保存工作簿
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### 另请参见

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


