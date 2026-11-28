---
title: "BarEquationNode.BarPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BarEquationNode özelliği. Bu öznitelik, çubuk nesnesindeki çubuğun konumunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Bu öznitelik, çubuk nesnesindeki çubuğun konumunu belirtir.

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem şekli ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklem düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Bir çubuk denklem düğümü oluşturun
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Çubuk konumunu Üst olarak ayarlayın
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Çubuk için temel içeriği ekleyin
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Çalışma kitabını kaydedin
            workbook.Save("BarEquationDemo.xlsx");

            // Kaydedilen dosyayı doğrula
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


