---
title: "NaryEquationNode.IsHideSubscript"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NaryEquationNode özelliği. Alt sınırın gösterilip gösterilmeyeceği"
type: docs
url: /tr/net/aspose.cells.drawing.equations/naryequationnode/ishidesubscript/
---
## NaryEquationNode.IsHideSubscript property

Alt sınırın gösterilip gösterilmeyeceği

```csharp
public bool IsHideSubscript { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSubscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Gizli alt simgeyle bir Nary denklem düğümü oluştur
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSubscript = true; // Hide subscript
            node.IsHideSuperscript = false; // Show superscript

            // Alt simge ekle (gizlenecek)
            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            subText.Text = "1";

            // Üst simge ekle (görünecek)
            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            supText.Text = "5";

            // Taban ekle
            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            baseText.Text = "C";

            // Kaydet ve doğrula
            workbook.Save("NaryEquationDemo.xlsx");
            
            // Özellikleri doğrulamak için yeniden yükle
            Workbook loadedWorkbook = new Workbook("NaryEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode loadedNode = (NaryEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + loadedNode.NaryOperator);
            Console.WriteLine("IsHideSubscript: " + loadedNode.IsHideSubscript);
            Console.WriteLine("IsHideSuperscript: " + loadedNode.IsHideSuperscript);
        }
    }
}
```

### Ayrıca Bakınız

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


