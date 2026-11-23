---
title: "AccentEquationNode.AccentCharacter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AccentEquationNode 属性。此属性指定附加在重音函数基底上的组合变音符号的类型。默认的重音字符是 U0302。强烈建议使用属性 AccentType 来设置重音字符。如果在已知类型中找不到所需字符，请使用此属性设置。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

此属性指定附加在重音函数基部的组合变音标记的类型。默认的重音字符是 U+0302。强烈建议使用属性 AccentType 来设置重音字符。如果在已知类型中找不到所需的字符，请使用此属性设置。

```csharp
public string AccentCharacter { get; set; }
```

### 备注

需要注意的是，此属性仅接受一个字符，如果传入多个字符，只会接受第一个字符。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 向第一个工作表添加方程形状
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 获取方程节点并添加重音节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // 设置重音字符（此例为抑扬符）
            accentNode.AccentCharacter = "\u0302";

            // 为重音添加基文本
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // 保存工作簿
            workbook.Save("AccentEquationDemo.xlsx");

            // 通过重新加载来验证已保存的文件
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // 输出重音字符以演示该属性
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### 另请参见

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


