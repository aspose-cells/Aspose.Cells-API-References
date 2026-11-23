---
title: "枚举 EquationDelimiterShapeType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType 枚举。此枚举指定分隔符对象中分隔符的形状"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

此项指定分隔符对象中分隔符的形状。

```csharp
public enum EquationDelimiterShapeType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Centered | `0` | 分隔线在其内容的整个高度上居中。 |
| Match | `1` | 分隔线已被调整为恰好匹配其内容的高度。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加公式形状
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // 获取公式节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // 创建具有匹配形状类型的分隔符节点
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // 在分隔符内部添加内容
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // 保存工作簿
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


