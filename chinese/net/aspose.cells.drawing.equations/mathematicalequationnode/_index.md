---
title: "类 MathematicalEquationNode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.MathematicalEquationNode 类。此类指定方程或数学表达式。所有方程或数学表达式的数学文本均由此类包含"
type: docs
url: /zh/net/aspose.cells.drawing.equations/mathematicalequationnode/
---
## MathematicalEquationNode class

此类指定方程或数学表达式。所有方程或数学表达式的数学文本均由此类包含。

```csharp
public class MathematicalEquationNode : EquationNode
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
| override [Equals](../../aspose.cells.drawing.equations/mathematicalequationnode/equals/)(object) | 确定当前方程节点是否等于指定节点 |
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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassMathematicalEquationNodeDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个用于演示的新工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 创建两个 MathematicalEquationNode 实例用于比较
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;

                // 演示 Equals 方法
                bool areEqual = node1?.Equals((object)node2) ?? false;
                Console.WriteLine($"MathematicalEquationNode comparison result: {areEqual}");

                // 保存工作簿
                workbook.Save("MathematicalEquationNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MathematicalEquationNode: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


