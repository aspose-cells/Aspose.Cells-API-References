---
title: "RadicalEquationNode.IsDegHide"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadicalEquationNode-Eigenschaft. Ob der Grad der Radikale ausgeblendet werden soll"
type: docs
url: /de/net/aspose.cells.drawing.equations/radicalequationnode/isdeghide/
---
## RadicalEquationNode.IsDegHide property

Ob der Grad von Radikalen ausgeblendet werden soll.

```csharp
public bool IsDegHide { get; set; }
```

### Beispiele

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
            
            // Behoben: Verwenden Sie GetChild(0) und eine Nullprüfung anstelle der ChildCount-Eigenschaft
            EquationNode degreeNode = reloadedRadical.GetChild(0);
            EquationNode firstChildOfDegree = degreeNode.GetChild(0);
            Console.WriteLine("Degree node has child: " + (firstChildOfDegree != null));
        }
    }
}
```

### Siehe auch

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


