---
title: "类 EquationNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationNode 类。用于派生其他方程节点的抽象类"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class

用于派生其他方程节点的抽象类。

```csharp
public abstract class EquationNode : FontSetting
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | 获取当前节点的方程类型 |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | 返回此对象的字体。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | 获取字符的长度。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | 指定当前节点的父节点 |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | 获取字符的起始索引。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | 返回文本选项。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | 表示节点的类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CreateNode](../../aspose.cells.drawing.equations/equationnode/createnode/)(EquationNodeType, Workbook, EquationNode) | 创建指定类型的节点。 |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild_1)(EquationNode) | 在当前节点的子节点列表末尾插入指定节点。 |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild)(EquationNodeType) | 在当前节点的子节点列表末尾插入指定类型的节点。 |
| override [Equals](../../aspose.cells.drawing.equations/equationnode/equals/)(object) | 确定当前方程节点是否等于指定节点 |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | 返回当前节点子节点中指定索引处的节点。 |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | 在当前节点之后插入指定节点。 |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | 在当前节点之前插入指定的节点。 |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | 在当前节点的子节点列表中，在指定的索引位置插入指定类型的节点。 |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | 从父节点中移除自身。 |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | 移除当前节点的所有子节点。 |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild)(EquationNode) | 从当前节点的子节点中移除指定的节点。 |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild_1)(int) | 从当前节点的子节点中移除指定索引处的节点。 |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | 设置预设的 WordArt 样式。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | 将此等式转换为 LaTeX 表达式。 |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | 将此等式转换为 MathML 表达式。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加文本框并获取其索引
            int textBoxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "=A1+B1";
            
            // 从文本框获取方程节点
            EquationNode node = textBox.GetEquationParagraph();
            
            // 使用 ToString() 输出方程文本
            Console.WriteLine("Equation: " + node.ToString());
            
            // 通过设置新文本来修改方程
            textBox.Text = "=A1*B1";
            Console.WriteLine("Modified Equation: " + textBox.Text);
        }
    }
}
```

### 另请参见

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


