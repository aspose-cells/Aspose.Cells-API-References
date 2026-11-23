---
title: "类 EquationNodeParagraph"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationNodeParagraph 类。此类指定包含一个或多个 MathEquationNodeOMath 元素的数学段落。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnodeparagraph/
---
## EquationNodeParagraph class

此类指定一个包含一个或多个 MathEquationNode(OMath) 元素的数学段落。

```csharp
public class EquationNodeParagraph : EquationNode
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | 获取当前节点的方程类型（继承自 [`EquationNode`](../equationnode/)。） |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | 返回此对象的字体。（继承自 [`FontSetting`](../../aspose.cells/fontsetting/)。） |
| [Justification](../../aspose.cells.drawing.equations/equationnodeparagraph/justification/) { get; set; } | 这指定了数学段落的对齐方式（同一段落内相邻方程的系列）。数学段落可以是左对齐、右对齐、居中或整体居中。默认情况下，数学段落是整体居中。这意味着方程之间可以相互对齐，但整个方程组整体居中。 |
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
| override [Equals](../../aspose.cells.drawing.equations/equationnodeparagraph/equals/)(object) | 确定当前方程节点是否等于指定节点 |
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationNodeParagraphDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建一个形状来容纳方程段落
                var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

                // 从形状获取方程段落
                var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

                if (equationParagraph != null)
                {
                    // 显示默认对齐方式
                    Console.WriteLine($"Default Justification: {equationParagraph.Justification}");

                    // 将对齐方式改为左对齐
                    equationParagraph.Justification = EquationHorizontalJustificationType.Left;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // 将对齐方式改为居中
                    equationParagraph.Justification = EquationHorizontalJustificationType.Center;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // 保存工作簿
                    workbook.Save("EquationNodeParagraphDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("Failed to get EquationNodeParagraph from shape.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationNodeParagraph: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


