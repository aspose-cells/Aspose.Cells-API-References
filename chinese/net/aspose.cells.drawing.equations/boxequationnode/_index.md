---
title: "类 BoxEquationNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.BoxEquationNode 类。此类指定用于对方程组件进行分组的盒子函数"
type: docs
url: /zh/net/aspose.cells.drawing.equations/boxequationnode/
---
## BoxEquationNode class

此类指定 box 功能，用于对方程的组件进行分组。

```csharp
public class BoxEquationNode : EquationNode
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | 获取当前节点的方程类型（继承自 [`EquationNode`](../equationnode/)。） |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | 返回此对象的字体。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
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
| override [Equals](../../aspose.cells.drawing.equations/boxequationnode/equals/)(object) | 确定当前方程节点是否等于指定节点 |
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
    public class EquationsClassBoxEquationNodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 向第一个工作表添加方程文本框
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 从文本框获取方程节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // 添加盒子方程节点
            BoxEquationNode boxNode = (BoxEquationNode)mathNode.AddChild(EquationNodeType.Box);
            
            // 向盒子添加基节点
            EquationNode baseNode = boxNode.AddChild(EquationNodeType.Base);
            
            // 向基节点添加文本
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "==";

            // 保存工作簿
            string outputFile = "BoxEquationDemo.xlsx";
            workbook.Save(outputFile);

            Console.WriteLine("Equation with Box node created successfully. File saved to: " + outputFile);
        }
    }
}
```

### 另请参见

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


