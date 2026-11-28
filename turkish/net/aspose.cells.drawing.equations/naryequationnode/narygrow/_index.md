---
title: "NaryEquationNode.NaryGrow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NaryEquationNode özelliği. Bu öznitelik, belge seviyesindeki nary operatörlerin büyüme özelliğini belirtir. Kapalı olduğunda integral ve toplam gibi nary operatörler, operand yüksekliğine göre büyümez. Açık olduğunda nary operatör, operand yüksekliğine göre dikey olarak büyür."
type: docs
url: /tr/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Bu öznitelik, belge düzeyinde n-ary operatörlerin büyüme özelliğini belirtir. Kapalı olduğunda, integral ve toplam gibi n-ary operatörler, operand yüksekliğine göre büyümez. Açık olduğunda, n-ary operatör dikey olarak operand yüksekliğine uyacak şekilde büyür.

```csharp
public bool NaryGrow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Denklem şekli ekle
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Denklem düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // NaryGrow özelliği true olarak ayarlanmış bir nary operatör düğümü oluşturun
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Alt simge ekleyin (isteğe bağlı)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Üst simge ekleyin (isteğe bağlı)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Taban ekleyin (gerekli)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Çalışma kitabını kaydedin
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


