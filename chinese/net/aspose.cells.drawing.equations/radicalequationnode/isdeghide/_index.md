---
title: "RadicalEquationNode.IsDegHide"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RadicalEquationNode 属性。是否隐藏根号的指数"
type: docs
url: /zh/net/aspose.cells.drawing.equations/radicalequationnode/isdeghide/
---
## RadicalEquationNode.IsDegHide property

是否隐藏根式的次数。

```csharp
public bool IsDegHide { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class RadicalEquationNodePropertyIsDegHideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            TextBox textBox = worksheet.Shapes.AddEquation(0, 0, 0, 0, 200, 100);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            
            radicalNode.IsDegHide = true;
            
            EquationNode degNode = radicalNode.AddChild(EquationNodeType.Degree);
            TextRunEquationNode degText = (TextRunEquationNode)degNode.AddChild(EquationNodeType.Text);
            degText.Text = "3";
            
            EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            workbook.Save("RadicalEquationNodePropertyIsDegHideDemo_Out.xlsx");
            
            Workbook reloadedWorkbook = new Workbook("RadicalEquationNodePropertyIsDegHideDemo_Out.xlsx");
            TextBox reloadedTextBox = (TextBox)reloadedWorkbook.Worksheets[0].Shapes[0];
            RadicalEquationNode reloadedRadical = (RadicalEquationNode)reloadedTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);
                
            Console.WriteLine("Reloaded IsDegHide: " + reloadedRadical.IsDegHide);
            
            // 已修复：使用 GetChild(0) 并进行 null 检查，而不是使用 ChildCount 属性
            EquationNode degreeNode = reloadedRadical.GetChild(0);
            EquationNode firstChildOfDegree = degreeNode.GetChild(0);
            Console.WriteLine("Degree node has child: " + (firstChildOfDegree != null));
        }
    }
}
```

### 另请参见

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


