---
title: "EquationNode.EquationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode özelliği. Mevcut düğümün denklem tipini al"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/equationtype/
---
## EquationNode.EquationType property

Geçerli düğümün denklem tipini al

```csharp
public EquationNodeType EquationType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class EquationNodePropertyEquationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Drawing.TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Denklem yapısı oluştur
            Aspose.Cells.Drawing.Equations.EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Alt simge düğümü oluştur
            Aspose.Cells.Drawing.Equations.EquationNode subNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Sub);
            
            // Taban ve alt simge bileşenlerini ekle
            Aspose.Cells.Drawing.Equations.EquationNode baseNode = subNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            Aspose.Cells.Drawing.Equations.TextRunEquationNode baseText = (Aspose.Cells.Drawing.Equations.TextRunEquationNode)(baseNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text));
            baseText.Text = "Base";
            
            Aspose.Cells.Drawing.Equations.EquationNode subscriptNode = subNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Subscript);
            Aspose.Cells.Drawing.Equations.TextRunEquationNode subText = (Aspose.Cells.Drawing.Equations.TextRunEquationNode)(subscriptNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text));
            subText.Text = "Sub";

            // EquationType özelliğini doğrula
            Console.WriteLine("Main node type: " + mathNode.EquationType);
            Console.WriteLine("Subscript node type: " + subNode.EquationType);
            Console.WriteLine("Base component type: " + baseNode.EquationType);
            Console.WriteLine("Subscript component type: " + subscriptNode.EquationType);

            // Kalıcı olmayı doğrulamak için kaydet ve yeniden yükle
            workbook.Save("EquationTypeDemo.xlsx");
            workbook = new Workbook("EquationTypeDemo.xlsx");
            
            // Yüklenen denklem tiplerini doğrula
            Aspose.Cells.Drawing.TextBox loadedTextBox = (Aspose.Cells.Drawing.TextBox)workbook.Worksheets[0].Shapes[0];
            Aspose.Cells.Drawing.Equations.EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            Aspose.Cells.Drawing.Equations.SubSupEquationNode loadedSubNode = (Aspose.Cells.Drawing.Equations.SubSupEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Subscript node type: " + loadedSubNode.EquationType);
            Console.WriteLine("Base component type: " + loadedSubNode.GetChild(0).EquationType);
            Console.WriteLine("Subscript component type: " + loadedSubNode.GetChild(1).EquationType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


